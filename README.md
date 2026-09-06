# Django Again · To-Do Prototype

A Django learning repository containing project configuration and an early to-do application.

**Python · Django**

[Getting started](#getting-started) · [Repository guide](#repository-guide) · [Checks](#checks-and-review) · [Credits](#credits-and-reuse)

## What you can explore

- Django project in PROJ_NAME/.
- A todo application for exploring models and views.
- A local SQLite database snapshot.

> **Project notes:** A dependency manifest is not committed, and the todo app is not registered in INSTALLED_APPS. The settings header records Django 3.2.16; restore an appropriate development environment and app wiring before treating this as a complete to-do application.

## Getting started

Requires Git, Python, pip and a virtual environment. Dependency pins in older projects may need a compatible Python environment; this README does not upgrade them.

```bash
git clone https://github.com/SamOBrienOlinger/Django-Again.git
cd Django-Again
python3 -m venv .venv
source .venv/bin/activate
```

On Windows, activate the environment with `.venv\Scripts\Activate.ps1` instead.

**Dependency setup is incomplete:** no requirements file is committed. Identify and install the dependencies imported by the project before continuing. A dependency manifest is not committed, and the todo app is not registered in INSTALLED_APPS. The settings header records Django 3.2.16; restore an appropriate development environment and app wiring before treating this as a complete to-do application.

After resolving the project notes and configuring the local environment, use:

```bash
python manage.py check
python manage.py migrate
python manage.py runserver
```

Open [localhost:8000](http://localhost:8000). Stop the server with **Ctrl+C**. Use `python manage.py createsuperuser` in the same project directory if you need access to Django admin.

## Repository guide

| Path | Purpose |
| --- | --- |
| [manage.py](manage.py) | Django management commands |
| [PROJ_NAME/settings.py](PROJ_NAME/settings.py) | Django configuration |

## Checks and review

From the directory containing `manage.py`, run `python manage.py check` and `python manage.py test` after configuring an isolated development database. Inspect the test modules: scaffold `tests.py` files may contain no actual tests.

Generate fresh results from the revision you are working on; historical test reports describe earlier runs.

## Deployment

No current hosted endpoint is established by this README. A backend deployment needs a configured runtime and its own service settings; GitHub Pages cannot execute the server-side application.

## Credits and reuse

Learning resources and starter material: [Code Institute](https://codeinstitute.net/).

No repository-level licence file is present in this snapshot. This README does not grant additional reuse permissions. Check with the relevant rights holders before reusing code, written content or assets.

## Support

Repository maintained in [Sam O’Brien-Olinger’s GitHub account](https://github.com/SamOBrienOlinger). For a problem or suggested improvement, [open an issue](https://github.com/SamOBrienOlinger/Django-Again/issues) with the affected page or command, steps to reproduce, and expected behaviour.

[Back to top](#django-again--to-do-prototype)
