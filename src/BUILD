from os import environ

python_binary(
  name = 'ef-cf',
  source = 'ef-cf.py',
  dependencies = [
    ':boto3',
    ':ef-open-lib',
    ':ef-plugins',
    ':yaml'
  ]
 )

python_binary(
  name = 'ef-check-config',
  source = 'ef-check-config.py',
  dependencies = [
    ':boto3',
    ':ef-open-lib',
    ':ef-plugins'
  ]
)

python_binary(
  name = 'ef-generate',
  source = 'ef-generate.py',
  dependencies = [
    ':boto3',
    ':ef-open-lib',
    ':ef-plugins',
    ':yaml'
  ]
)

python_binary(
  name = 'ef-instanceinit',
  source = 'ef-instanceinit.py',
  dependencies = [
    ':boto3',
    ':ef-open-lib',
    ':ef-plugins',
    ':yaml'
  ]
)

python_binary(
  name = 'ef-password',
  source = 'ef-password.py',
  dependencies = [
    ':boto3',
    ':ef-open-lib',
    ':ef-plugins',
    ':yaml'
  ]
)

python_binary(
  name = 'ef-resolve-config',
  source = 'ef-resolve-config.py',
  dependencies = [
    ':boto3',
    ':ef-open-lib',
    ':ef-plugins',
    ':yaml'
  ]
)

python_binary(
  name = 'ef-version',
  source = 'ef-version.py',
  dependencies = [
    ':boto3',
    ':ef-open-lib',
    ':ef-plugins',
    ':yaml'
  ]
)

python_requirement_library(
  name = 'boto3',
  requirements = [
    python_requirement("boto3")
  ]
)

python_requirement_library(
  name = 'yaml',
  requirements = [
    python_requirement("pyyaml")
  ]
)

python_library(
  name = 'ef-open-lib',
  sources = globs('ef_*.py')
)

python_library(
  name = 'ef-plugins',
  dependencies = [
    environ["EF_SITE_REPO"]+":plugins",
    environ["EF_SITE_REPO"]+":plugin_modules"
  ]
)
