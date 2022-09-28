# project_settings

Configures base settings for a tilt project

<br/>

# Usage

```python
project_setup(
  min_k8s_version: str, # Required
  min_tilt_version: str, # Defaults to 0.38.0
  use_dotenv: bool, # Defaults to True
  dotenv_file: str # defaults to project_root_dir/.env
)
```

```python
v1alpha1.extension_repo(name='voidstack', url='https://github.com/voidstack-io/tilt-extensions')
v1alpha1.extension(name='project_setup', repo_name='voidstack', repo_path='project_setup')
load('ext://project_setup', 'project_setup')

# Simple
project_setup('1.24.0')
# With alternative minimum tilt version
project_setup('1.24.0', '0.37.0')
# Without dotenv setup
project_setup('1.24.0', use_dotenv=False)
# Use an alternative dotenv file
project_setup('1.24.0', dotenv_file='.env.local')
```
