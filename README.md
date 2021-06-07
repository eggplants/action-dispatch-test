# action-dispatch-test

[![Workflow dispatch](https://github.com/eggplants/action-dispatch-test/actions/workflows/workflow_disp.yml/badge.svg)](https://github.com/eggplants/action-dispatch-test/actions/workflows/workflow_disp.yml)

↕↕↕↕↕↕↕↕↕↕↕

[![Repo dispatch](https://github.com/eggplants/action-dispatch-test/actions/workflows/rep_disp.yml/badge.svg)](https://github.com/eggplants/action-dispatch-test/actions/workflows/rep_disp.yml)

- Call another Action from an Action, wait for it to finish, and get the result
- Actionから別Actionを呼び出し、終了を待機・結果を取得する


## Requirement

- Set PAT with `repo` to `Secrets`
  - See: [peter-evans/repository-dispatch](https://github.com/peter-evans/repository-dispatch#token)

## Screenshot

<https://github.com/eggplants/action-dispatch-test/actions/runs/915592304>

![image](https://user-images.githubusercontent.com/42153744/121058407-40094480-c7fb-11eb-8515-a5c1b753a970.png)

## Tips

<https://docs.github.com/en/rest/reference/checks#create-a-check-run>

### `status`

- `queued`, `in_progress`, or `completed`

### `conclusion`

Note: It provides after status turns into `completed_at` `completed`

- `action_required`, `cancelled`, `failure`, `neutral`, `success`, `skipped`, `stale`, or `timed_out`
