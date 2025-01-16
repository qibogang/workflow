The repository **qiboteam/workflow** is a collection of **reusable workflows** used
across the qiboteam organization. The workflows are availaible in the folder
[`github/workflows`](https://github.com/qiboteam/workflows/tree/v2/.github/workflows).

# Available workflows

- [`test`](./workflows/test.md)
- [`wheels`](./workflows/wheels.md)
- [`docs`](./workflows/docs.md)
- [`latest-stable`](./workflows/latest-stable.md)
- [`selfhosted`](./workflows/selfhosted.md)

## How to use a reusable workflow ?

If you want to use the **reusable workflow** `docs.yml`, all you have to do is to add
the `uses` keyword in a job of your workflow, for example

```yaml
jobs:
  calling-job:
    uses: qiboteam/workflows/.github/workflows/docs.yml@main
    with:
      python-version: 3.11
```

# Actions

For workflows developers: some workflows' building blocks are split as individual
[actions](./actions).
