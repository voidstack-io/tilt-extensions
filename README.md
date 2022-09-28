# Tilt.dev Extensions

## How to use this extension repository

To use extensions from this repo add the following to the top of you `Tilt` file

```python
# Add custom extension repo from https://github.com/voidstack-io/tilt-extensions
v1alpha1.extension_repo(name='voidstack', url='https://github.com/voidstack-io/tilt-extensions')
# Add extensions from voidstack repo. Replace `extension_name` and `extension_repo_path` with the values for the extension you are adding
v1alpha1.extension(name='extension_name', repo_name='voidstack', repo_path='extension_repo_path')
# Load the extension into the tilt file
load('ext://extension_name', 'extension_function_name')
```

---

## Extensions List
