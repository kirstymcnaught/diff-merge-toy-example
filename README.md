This is a really simple repo set up to validate git difftool/mergetool setups.

Once you have a difftool/mergetool set up, you can test your config by cloning this repository and following the instructions below.

> git clone <this_repo>
> cd diff-merge-toy-example

## Testing your difftool
> git checkout kirstyBranch
> git difftool head    # show diff against previous commit on kirstyBranch

If everything is set up okay, your favourite difftool should be launched and show the expected diff.

## Testing your mergetool 

> git merge origin/alastairBranch

At this point git should say:
> Auto-merging myfile.txt
> CONFLICT (content): Merge conflict in myfile.txt
> Automatic merge failed; fix conflicts and then commit the result.

Now launch your mergetool to resolve conflicts:
> git mergetool 

If everything is set up okay, your favourite mergetool should be launched and show the expected diffs/conflicts.
