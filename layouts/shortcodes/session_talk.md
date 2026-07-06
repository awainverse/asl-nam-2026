{{- range $index, $page := (where (.Get "pagelist") ".Params.speaker" .speaker ) }}
    {{ .Render "summary" }}
{{- end }}