Git Team Sync Workflow



1\. What did the rejected push say, and why?



The rejected push said non-fast-forward and fetch first. It happened because the remote branch had commits that my local branch did not have, so Git rejected the push to prevent overwriting other changes.



2\. How was conflict resolution different between merge and rebase?



With merge, I resolved the conflict and created a merge commit that joined both histories. With rebase, I resolved the conflict while replaying my commit on top of the updated branch, keeping the history more linear without creating another merge commit.



3\. What habit would avoid both rejected pushes?



I should always fetch or pull the latest changes before starting work and before pushing, especially when other teammates are working on the same branch.



4\. On a shared team branch, would you default to merge or rebase, and why?



I would default to merge on a shared team branch because it preserves the shared history and does not rewrite commits that other teammates may already have. I would use rebase mainly on my own local branch before sharing it.



