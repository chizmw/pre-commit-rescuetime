# Pre-commit git hooks

Git hooks to integrate with [pre-commit](http://pre-commit.com).

## Table of contents

- [Configure pre-commit](#configure-pre-commit)
- [Available hooks](#available-hooks)
  * [`rescuetime-highlight`](#rescuetime-highlight)

## Configure pre-commit

Add this to your `.pre-commit-config.yaml`:

```yaml
-   repo: https://github.com/chiselwright/pre-commit-rescuetime
    rev: v0.0.2
    hooks:
    -   id: rescuetime-highlight
```

## Available hooks

### `rescuetime-highlight`

**What it does**

Posts a highlight to Rescuetime using the [API](https://www.rescuetime.com/apidoc#highlights-feed-reference)

**Requirements**

You must have set `RESCUETIME_API_KEY` in your environment.

This must be a valid Rescuetime API key; you can manage your keys [here](https://www.rescuetime.com/anapi/manage)
