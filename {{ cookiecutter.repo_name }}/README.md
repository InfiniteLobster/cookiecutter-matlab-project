# {{ cookiecutter.project_name }}

{{ cookiecutter.description }}

{% if cookiecutter.is_package == 'yes' %}
> **Note:** This is a MATLAB package. Use with `{{ cookiecutter.project_name }}.functionName()` syntax.
{% endif %}

## Installation

```bash
git clone https://github.com/YOUR-USERNAME/{{ cookiecutter.repo_name }}.git
```

Add to MATLAB path:
```matlab
addpath('src{% if cookiecutter.is_package == 'no' %}/{{ cookiecutter.project_name }}{% endif %}');
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

- MATLAB R20XXa or later

## Author

{{ cookiecutter.author_name }}

## Version

{{ cookiecutter.version }} (Created: {% now 'utc', '%Y-%m-%d' %})

## License

MIT License

