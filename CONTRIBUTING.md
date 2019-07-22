# Making contributions

## Markdown
All files in the pulsar-translation repository are written in [Markdown](https://www.markdownguide.org/). If you do not know how to use Markdown, learn how to [get started](https://www.markdownguide.org/getting-started).


## Workflow

### Step 1: Fork

1. Visit https://github.com/apache/pulsar-translation
2. Click `Fork` button (top right) to establish a cloud-based fork.

### Step 2: Clone fork to local machine

Create your clone.

```sh
$ cd $working_dir
$ git clone https://github.com/$user/pulsar-translation
```

Set your clone to track upstream repository.

```sh
$ cd $working_dir/pulsar-translation
$ git remote add upstream https://github.com/apache/pulsar-translation.git
```

Use the `git remote -v` command, you find the output looks as follows:

```
origin    https://github.com/$user/pulsar-translation.git (fetch)
origin    https://github.com/$user/pulsar-translation.git (push)
upstream  https://github.com/apache/pulsar-translation (fetch)
upstream  https://github.com/apache/pulsar-translation (push)
```

### Step 3: Keep your branch in sync

Get your local master up to date.

```sh
$ cd $working_dir/pulsar-translation
$ git checkout master
$ git fetch upstream
$ git rebase upstream/master
$ git push origin master 
```

### Step 4: Create your branch

Branch from master.

```sh
$ git checkout -b myfeature
```

### Step 5: Edit the code

You can now edit the code on the `myfeature` branch.


### Step 6: Commit

Commit your changes.

```sh
$ git add <filename>
$ git commit -m "$add a comment"
```

Likely you'll go back and edit-build-test in a few cycles. 

The following commands might be helpful for you.

```sh
$ git add <filename> (used to add one file)
git add -A (add all changes, including new/delete/modified files)
git add -a -m "$add a comment" (add and commit modified and deleted files)
git add -u (add modified and deleted files, not include new files)
git add . (add new and modified files, not including deleted files)
```

### Step 7: Push

When your commit is ready for review (or just to establish an offsite backup of your work), push your branch to your fork on `github.com`:

```sh
$ git push origin myfeature
```

### Step 8: Create a pull request

1. Visit your fork at https://github.com/$user/pulsar-translation (replace `$user` obviously).
2. Click the `Compare & pull request` button next to your `myfeature` branch.

### Step 9: Get a code review

Once you open your pull request, at least two reviewers will participate in reviewing. Those reviewers will conduct a thorough code review, looking for correctness, bugs, opportunities for improvement, documentation and comments, and style.

Commit changes made in response to review comments to the same branch on your fork.

Very small PRs are easy to review. Very large PRs are very difficult to review.
