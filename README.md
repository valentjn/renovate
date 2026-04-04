<!-- Copyright (C) 2026 Julian Valentin
   -
   - This Source Code Form is subject to the terms of the Mozilla Public
   - License, v. 2.0. If a copy of the MPL was not distributed with this
   - file, You can obtain one at https://mozilla.org/MPL/2.0/.
   -->

# `valentjn/renovate`

This repository contains a GitHub Actions workflow that runs Renovate on select `valentjn` repositories. The workflow is run weekly and can be triggered manually.

## Adding a Repository

1. Make sure that pull requests are enabled in the settings of the repository to be added (can be set to collaborator only). Otherwise, Renovate will error.
2. Create `.github/renovate.json` in the repository to be added with the following contents:

   <!-- prettier-ignore -->
   ```json
   {
       "$schema": "https://docs.renovatebot.com/renovate-schema.json",
       "extends": ["github>valentjn/renovate"]
   }
   ```

3. Add the repository to [`self-hosted.json`](self-hosted.json) in this repository.
