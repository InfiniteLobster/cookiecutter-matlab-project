# {{ cookiecutter.project_name }}

{{ cookiecutter.description }}

{% if cookiecutter.is_package == 'yes' %}
> **Note:** This is a MATLAB package. Use with `{{ cookiecutter.project_name }}.functionName()` syntax.
{% endif %}

## Installation

```bash
git clone <link to repo>
```

## Usage

{% if cookiecutter.is_package == 'yes' %}
```matlab
result = {{ cookiecutter.project_name }}.main();
```
{% else %}
```matlab
result = main();
```
{% endif %}


## Examples

See the `examples/` directory for usage examples.

## Testing

```matlab
runtests('tests')
```

## Requirements

- MATLAB R20{{cookiecutter.matlab_version}} or later

## Author

{{ cookiecutter.author_name }}

## Version

{{ cookiecutter.version }} (Created: {% now 'utc', '%Y-%m-%d' %})

## License

MIT License

