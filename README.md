# jenkins_simple_assert_tests

Homework: Jenkins + pytest + Allure (qa-guru Python Base).

## Local run

```bash
python3 -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
pytest
allure serve allure-results
```

## Jenkins

- View: https://jenkins.autotests.cloud/view/python_students/
- Label: `python`
- Branch: `*/main`
- Build step: venv + pip + pytest
- Post-build: Allure Report → `allure-results`
