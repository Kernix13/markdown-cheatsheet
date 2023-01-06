# Shields io

[Shields.io](https://shields.io/)

Below are all the Shields.io badges for GitHub.

## Build

> Cirrus CI is a modern _Continuous Integration_ system built for the era of cloud computing. Cirrus CI supports Linux, Windows, macOS and FreeBSD environments...

Continuous Improvement badges

1. Cirrus CI - Base Branch build status: `/cirrus/github/:user/:repo`
1. Cirrus CI - Base Specific build status:`/cirrus/github/:user/:repo/:branch`
1. Cirrus CI - Base Specific task build status`/cirrus/github/:user/:repo?task=build_docker`
1. Cirrus CI - task & script build:`/cirrus/github/:user/:repo?script=test&task=build_docker`

Actions badges

1. GitHub Workflow status: `/github/actions/workflow/status/:user/:repo/:workflow+?branch=main`
1. GitHub Workflow status (with event): `/github/actions/workflow/status/:user/:repo/:workflow+?branch=main&event=push`

Branch, tags, and PR checks (good for beginners maybe?):

1. GitHub branch checks state: `/github/checks-status/:user/:repo/:ref`
1. GitHub commit checks state: `/github/checks-status/:user/:repo/:ref`
1. GitHub tags checks state: `/github/checks-status/:user/:repo/:ref`
1. GitHub pull request checks state: `/github/status/s/pulls/:user/:repo/:number`
1. GitHub pull request check context: `/github/status/contexts/pulls/:user/:repo/:number`

Scrutinizer build (?)

1. Scrutinizer build (GitHub/BitBucket): `/scrutinizer/build/:vcs/:user/:repo/:branch?`

## Code Coverage

No clue what these are:

1. nycrc config on GitHub: `/nycrc/:user/:repo?config=.nycrc&preferredThreshold=lines`
1. Scrutinizer coverage (GitHub/BitBucket): `/scrutinizer/coverage/:vcs/:user/:repo/:branch?`

## Test Results

I'm doing a search on _GitHub_ and there are no shields on this page specifically for GitHub. It appears they are for the following testing software:

1. AppVeyor
1. **Azure**: see this one in job openings a lot
1. **Jenkins**: also a common one
1. Sonar
1. TAS
1. Testspace

> No Puppeteer?

## Analysis

Language and search (These would be good for a beginners repo):

1. **GitHub language count**: `/github/languages/count/:user/:repo`
1. **GitHub search hit counter**: `/github/search/:user/:repo/:query`
1. **GitHub top language**: `/github/languages/top/:user/:repo`

Scrutinizer & Snyk (?):

1. Scrutinizer code quality (GitHub/BitBucket): `/scrutinizer/quality/:vcs/:user/:repo/:branch?`
1. Snyk Vulnerabilities for GitHub repo: `/snyk/vulnerabilities/github/:user/:repo`
1. Snyk Vulnerabilities for GitHub repo (specific manifest): `/snyk/vulnerabilities/github/:user/:repo/:manifestFilePath`
1.

## Chat

Badges for:

1. **Discord**: 
   1. [general](/discord/:serverId),
   1. [topics](/discourse/topics?server=https%3A%2F%2Fmeta.discourse.org)
   1. [users](/discourse/users?server=https%3A%2F%2Fmeta.discourse.org)
   1. [posts](/discourse/posts?server=https%3A%2F%2Fmeta.discourse.org)
   1. [likes](/discourse/likes?server=https%3A%2F%2Fmeta.discourse.org)
   1. [status](/discourse/status?server=https%3A%2F%2Fmeta.discourse.org)
2. Glitter: skip
3. Matrix: skip
4. Stack Exchange
   1. [monthly questions]((/stackexchange/:stackexchangesite/qm/:query))
   1. [reputation](/stackexchange/:stackexchangesite/r/:query)
   1. [questions](/stackexchange/:stackexchangesite/t/:query)

## Dependencies

Depfu (?):

1. GitHub Pipenv locked dependency version: `/github/pipenv/locked/dependency-version/:user/:repo/:kind?/:packageName`
1. GitHub Pipenv locked dependency version (branch): `/github/pipenv/locked/dependency-version/:user/:repo/:kind?/:packageName/:branch`
1. Libraries.io dependency status for GitHub repo: `/librariesio/github/:user/:repo`

## Size

Some of these would be good for a beginner's repo:

1. GitHub code size in bytes: `/github/languages/code-size/:user/:repo`
1. **GitHub repo file count**: `/github/directory-file-count/:user/:repo`
1. GitHub repo file count (custom path): `/github/directory-file-count/:user/:repo/:path`
1. GitHub repo directory count: `/github/directory-file-count/:user/:repo?type=dir`
1. GitHub repo directory count (custom path): `/github/directory-file-count/:user/:repo/:path?type=dir`
1. **GitHub repo file count (file type)**: `/github/directory-file-count/:user/:repo?type=file`
1. GitHub repo file count (custom path & file type): `/github/directory-file-count/:user/:repo/:path?type=file`
1. **GitHub repo file count (fiel extension)**: `/github/directory-file-count/:user/:repo/:path?extension=js&type=file`
1. GitHub repo size: `/github/repo-size/:user/:repo`
1. GitHub repo file size in bytes: `/github/size/:user/:repo/:path*`
1. GitHub repo file size in bytes on a specified ref (branch/commit/tag): `/github/size/:user/:repo/:path*?branch=master`

## Downloads

Only good for repos that have a release(s)

1. GitHub all releases: `/github/downloads/:user/:repo/total`
1. GitHub release (latest by date): `/github/downloads/:user/:repo/:tag/total`
1. GitHub release (latest by SemVer): `/github/downloads/:user/:repo/:tag/total?sort=semver`
1. GitHub release (latest by date including pre-release): `/github/downloads-pre/:user/:repo/:tag/total`
1. GitHub release (latest by SemVer including pre-releases): `/github/downloads-pre/:user/:repo/:tag/total?sort=semver`
1. GitHub release (by tag): `/github/downloads/:user/:repo/:tag/total`
1. GitHub release (latest by date & asset): `/github/downloads/:user/:repo/:tag/:assetName`
1. GitHub release (latest by SemVer & asset): `/github/downloads/:user/:repo/:tag/:assetName?sort=semver`
1. GitHub release (latest by date & asset including pre-releases): `/github/downloads-pre/:user/:repo/:tag/:assetName`
1. GitHub release (latest by SemVer & asset including pre-releases): `/github/downloads-pre/:user/:repo/:tag/:assetName?sort=semver`
1. jsDeliver hits (GitHub): `/jsdelivr/gh/:period/:user/:repo`

## Funding

1. GitHub sponsors: `/github/sponsors/:user`

## Issue Tracking

Add these if you have issues and/or PRs.

Varied:

1. **GitHub commit merge status**: `/github/commit-status/:user/:repo/:branch/:commit`
1. GitHub Hacktoberfest combined status: `/github/hacktoberfest/:year/:user/:repo`
1. GitHub Hacktoberfest combined status (suggestion label override): `/github/hacktoberfest/:year/:user/:repo?suggestion_label=help%20wanted`
1. **GitHub issue/pull request detail**: `/github/:issueKind/detail/:property/:user/:repo/:number`
1. GitHub issue custom search: `/github/issues-search?query=repo%3Abadges%2Fshields%20is%3Aclosed%20label%3Abug%20author%3Aapp%2Fsentry-io`
1. GitHub issue custom search in repo: `/github/issues-search/:user/:repo?query=is%3Aclosed%20label%3Abug%20author%3Aapp%2Fsentry-io`
1. **Github labels**: `/github/labels/:user/:repo/:name`
1. Github milestone: `github/milestones/:variant/:user/:repo/:number`
1. Github milestones: `/github/milestones/:variant/:user/:repo`

Issues:

1. **GitHub issues**: `/github/issues/:user/:repo`
1. GitHub issues: `/github/issues-raw/:user/:repo`
1. **GitHub issues by label**: `/github/issues/:user/:repo/:label`
1. GitHub issues by label: `/github/issues-raw/:user/:repo/:label`
1. **GitHub closed issues**: `/github/issues-closed/:user/:repo`
1. GitHub closed issues: `/github/issues-closed-raw/:user/:repo`
1. **GitHub closed issues by label**: `/github/issues-closed/:user/:repo/:label`
1. GitHub closed issues by label: `/github/issues-closed-raw/:user/:repo/:label`

Pull requests:

1. GitHub pull requests: `/github/issues-pr/:user/:repo`
1. GitHub pull requests: `/github/issues-pr-raw/:user/:repo`
1. GitHub closed pull requests: `/github/issues-pr-closed/:user/:repo`
1. GitHub closed pull requests: `/github/issues-pr-closed-raw/:user/:repo`
1. GitHub pull requests by label: `/github/issues-pr/:user/:repo/:label`
1. GitHub pull requests by label: `/github/issues-pr-raw/:user/:repo/:label`
1. GitHub closed pull requests by label: `/github/issues-pr-closed/:user/:repo/:label`
1. GitHub closed pull requests by label: `/github/issues-pr-closed-raw/:user/:repo/:label`

## License

1. **GitHub**: `/github/license/:user/:repo`

## Rating

Not sure about where these ratings are coming from but the options are:

1. Mozilla Add-on
1. AUR votes
1. Chrome web store
1. Docker
1. Greasy fork
1. JetBrains Plugins
1. Libraries.io
1. Open VSX
1. Ore
1. Package gist
1. Pub
1. Puppet Forge
1. Plugin on redmine.org
1. Spiget
1. Stream
1. Vaadin Directory
1. **Visual Studio Marketplace**
1. **WordPress theme**
1. **WordPress plugin**

## Social

> These are all good (except Org stars)!!!

1. **GitHub gist stars**: `/github/gist/stars/:gistId`
1. **GitHub followers**: `/github/followers/:user?label=Follow`
1. **GitHub forks**: `/github/forks/:user/:repo?label=Fork`
1. **GitHub repo stars**: `/github/stars/:user/:repo?style=social`
1. **GitHub user's stars**: `/github/stars/:user?affiliations=OWNER%2CCOLLABORATOR`
1. GitHub Org's stars: `/github/stars/:org`
1. **GitHub watchers**: `/github/watchers/:user/:repo?label=Watch`

## Version

This section is for when you have a pro version of code or something where you have versions, releases, etc. I'm skipping this one because it definitely does not apply to me. But go to [Shields.io Version](https://shields.io/category/version) to see the list for yourself. Options:

1. go.mod
1. lerna
1. Manifest version
1. package.json version
1. R package version
1. release
1. GitHub tag SemVer
1. **GitHub tag (latest by date)**: `/github/v/tag/:user/:repo`

## Platform & Version Support

Skip if you are a newbie:

1. GitHub package.json dependency version (prod): `/github/package-json/dependency-version/:user/:repo/:packageName`
1. GitHub package.json dependency version (dev on branch): `/github/package-json/dependency-version/:user/:repo/dev/:scope?/:packageName/:branch*`
1. GitHub package.json dependency version (subfolder): `	/github/package-json/dependency-version/:user/:repo/:packageName?filename=packages%2Fchar-width-table-builder%2Fpackage.json`
1. GitHub Pipenv locked Python version: `/github/pipenv/locked/python-version/:user/:repo`
1. GitHub Pipenv locked Python version (branch): `/github/pipenv/locked/python-version/:user/:repo/:branch`

## Monitoring

Nothing GitHub specific and not for beginners - categories are:

1. Chromium
1. Mozilla
1. NodePing
1. PingPong
1. Security Headers
1. Uptime Robot

## Activity

> A lot of these look good!

Various:

1. **GitHub contributors** (<ins>via allcontributors.org</ins>): `/github/all-contributors/:user/:repo/:branch*`
1. GitHub release date: `/github/release-date/:user/:repo`
1. GitHub (Pre-)release date: `/github/release-date-pre/:user/:repo`
1. GitHub release date published_at: `/github/release-date/:user/:repo?display_date=published_at`

Commits:

1. **GitHub gist last commit**: `/github/gist/last-commit/:gistId`
1. **GitHub commit activity**: `/github/commit-activity/:interval/:user/:repo`
1. **GitHub commit activity (branch)**: `/github/commit-activity/:interval/:user/:repo/:branch*`
1. GitHub commits diff between...: `/github/commits-difference/:user/:repo?base=1.60.0&head=82f2db7`
1. GitHub commits since tagged version: `/github/commits-since/:user/:repo/:version/:branch*`
1. GitHub commits since tagged version (branch): `/github/commits-since/:user/:repo/:version/:branch*`
1. GitHub commits since latest release (by date): `/github/commits-since/:user/:repo/:version/:branch*`
1. GitHub commits since latest release (by date) for a branch: `/github/commits-since/:user/:repo/:version/:branch*`
1. GitHub commits since...: `/github/commits-since/:user/:repo/:version/:branch*?include_prereleases`
1. GitHub commits since... SemVeer: `/github/commits-since/:user/:repo/:version/:branch*?sort=semver`
1. GitHub commits since...: SKIP
1. **GitHub commits contributors**: `/github/:variant/:user/:repo`
1. **GitHub last commit**: `/github/last-commit/:user/:repo`
1. **GitHub last commit (branch)**: `/github/last-commit/:user/:repo/:branch`
1. **GitHub last commit (by commiter)**: `/github/last-commit/:user/:repo?display_timestamp=committer`

## Other

1 or 2 beginner badges in this section:

1. **GitHub deployments**: `/github/deployments/:user/:repo/:environment`
1. **GitHub discussions**: `/github/discussions/:user/:repo`
1. GitHub manifest.json dynamic: `/github/manifest-json/:key/:user/:repo`
1. GitHub manifest.json dynamic: `/github/manifest-json/:key/:user/:repo/:branch`
1. GitHub manifest.json dynamic (path): `/github/manifest-json/:key/:user/:repo?filename=extension%2Fmanifest.json`
1. GitHub manifest.json dynamic (path): `/github/manifest-json/:key/:user/:repo/:branch?filename=extension%2Fmanifest.json`
1. GitHub package.json dynamic: `/github/package-json/:key/:user/:repo`
1. GitHub package.json dynamic: `/github/package-json/:key/:user/:repo/:branch`