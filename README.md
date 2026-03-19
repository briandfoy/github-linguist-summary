# github-linguist-summary

I wanted to see a matrix of the [github-linguist](https://github.com/github-linguist/linguist)
results for all of my repos, so I threw this together.

	% cpan Mojolicious   # the only Perl thing you need
	% perl github-linguist-summary

The first time you call this, or after you delete the JSON cache file in the run
directory, this grabs a ton of data from GitHub.

From that data, this program outputs a text summary. There's some example
output in [example.txt](example.txt).

## When github-linguist guesses wrong

You can adjust what *github-linguist* does by adding hints to *.gitattributes* then commit that
file. The *github-linguist* program only looks at files committed to the repo, so uncommitted
changes to *.gitattributes* have no effect.

## You're on your own

This is something I threw together in an hour to track down a problem with my GitHub profile.
If you want to use it, it's probably best that you just steal it and do whatever you want.

## Further reading

* [github-linguist](https://github.com/github-linguist/linguist)

