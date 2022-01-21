# cookiecutter-kicad-project

## Git filters for better KiCad workflow

From [Massaging your git for kicad](https://jnavila.github.io/plotkicadsch/).

```bash
git config --global filter.kicad_project.clean "sed -E 's/^update=.*$/update=Date/'"
git config --global filter.kicad_project.smudge cat
git config --global filter.kicad_sch.clean "sed -E s/#('PWR|FLG)[0-9]+/#\1?/'"
git config --global filter.kicad_sch.smudge cat
```
