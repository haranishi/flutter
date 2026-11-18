# Local Flutter review snapshots

These three patches preserve exploratory changes in local review checkouts.
The Router patches are alternatives. The first includes an intentional
reversal of production behavior used during review.

| Patch | Base commit | Changed files |
| --- | --- | ---: |
| [194172-tree-sliver.patch](194172-tree-sliver.patch) | `b91da7005e292c6982342b5cacabf928ebe12cf9` | 2 |
| [194173-router-review.patch](194173-router-review.patch) | `9acd9b7e4f0281d4be5a907842deca9b683f7eb4` | 5 |
| [194173-router-review2.patch](194173-router-review2.patch) | `9acd9b7e4f0281d4be5a907842deca9b683f7eb4` | 3 |

To restore a snapshot, create a detached worktree at its base commit and
apply that patch with `git apply --binary /path/to/the.patch` from the worktree.
All changed files were compared byte-for-byte after applying each patch to
an independent Git index.

Original upstream reviews: [TreeSliver #194172](https://github.com/flutter/flutter/pull/194172)
and [Router #194173](https://github.com/flutter/flutter/pull/194173).
