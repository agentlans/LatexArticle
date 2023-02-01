.PHONY: all clean
all: {{ cookiecutter.project_slug }}.pdf

{{ cookiecutter.project_slug }}.pdf : {{ cookiecutter.project_slug }}.tex {% if cookiecutter.bibliography == 'y' %} {{-cookiecutter.bib_file-}}{% endif %}
	pdflatex $^
	{% if cookiecutter.bibliography == 'y' -%}
	biber {{ cookiecutter.project_slug }}
	pdflatex $^
	pdflatex $^
{%- endif %}

view: {{ cookiecutter.project_slug }}.pdf
	evince $^

clean:
	rm -f {{ cookiecutter.project_slug }}.pdf *.log *.aux

