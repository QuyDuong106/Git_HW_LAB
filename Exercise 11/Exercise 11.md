* Final Exercise - Using the GitHub API

1. Get a Github Users
```
C:\Users\D U O N G\advanced-git-exercises>curl "https://api.github.com/users/QuyDuong106"
{
  "login": "QuyDuong106",
  "id": 54212949,
  "node_id": "MDQ6VXNlcjU0MjEyOTQ5",
  "avatar_url": "https://avatars.githubusercontent.com/u/54212949?v=4",
  "gravatar_id": "",
  "url": "https://api.github.com/users/QuyDuong106",
  "html_url": "https://github.com/QuyDuong106",
  "followers_url": "https://api.github.com/users/QuyDuong106/followers",
  "following_url": "https://api.github.com/users/QuyDuong106/following{/other_user}",
  "gists_url": "https://api.github.com/users/QuyDuong106/gists{/gist_id}",
  "starred_url": "https://api.github.com/users/QuyDuong106/starred{/owner}{/repo}",
  "subscriptions_url": "https://api.github.com/users/QuyDuong106/subscriptions",
  "organizations_url": "https://api.github.com/users/QuyDuong106/orgs",
  "repos_url": "https://api.github.com/users/QuyDuong106/repos",
  "events_url": "https://api.github.com/users/QuyDuong106/events{/privacy}",
  "received_events_url": "https://api.github.com/users/QuyDuong106/received_events",
  "type": "User",
  "site_admin": false,
  "name": null,
  "company": null,
  "blog": "",
  "location": null,
  "email": null,
  "hireable": null,
  "bio": null,
  "twitter_username": null,
  "public_repos": 7,
  "public_gists": 0,
  "followers": 0,
  "following": 0,
  "created_at": "2019-08-17T14:45:47Z",
  "updated_at": "2023-09-01T09:20:10Z"
}
```

2. What's Our Most Popular Repo?
```
C:\Users\D U O N G\advanced-git-exercises>curl -s "https://api.github.com/search/repositories?q=user:QuyDuong106&sort=stars&per_page=1"
{
  "total_count": 7,
  "incomplete_results": false,
  "items": [
    {
      "id": 683990064,
      "node_id": "R_kgDOKMTcMA",
      "name": "OPENCV_Python",
      "full_name": "QuyDuong106/OPENCV_Python",
      "private": false,
      "owner": {
        "login": "QuyDuong106",
        "id": 54212949,
        "node_id": "MDQ6VXNlcjU0MjEyOTQ5",
        "avatar_url": "https://avatars.githubusercontent.com/u/54212949?v=4",
        "gravatar_id": "",
        "url": "https://api.github.com/users/QuyDuong106",
        "html_url": "https://github.com/QuyDuong106",
        "followers_url": "https://api.github.com/users/QuyDuong106/followers",
        "following_url": "https://api.github.com/users/QuyDuong106/following{/other_user}",
        "gists_url": "https://api.github.com/users/QuyDuong106/gists{/gist_id}",
        "starred_url": "https://api.github.com/users/QuyDuong106/starred{/owner}{/repo}",
        "subscriptions_url": "https://api.github.com/users/QuyDuong106/subscriptions",
        "organizations_url": "https://api.github.com/users/QuyDuong106/orgs",
        "repos_url": "https://api.github.com/users/QuyDuong106/repos",
        "events_url": "https://api.github.com/users/QuyDuong106/events{/privacy}",
        "received_events_url": "https://api.github.com/users/QuyDuong106/received_events",
        "type": "User",
        "site_admin": false
      },
      "html_url": "https://github.com/QuyDuong106/OPENCV_Python",
      "description": "OpenCV homework and learning ",
      "fork": false,
      "url": "https://api.github.com/repos/QuyDuong106/OPENCV_Python",
      "forks_url": "https://api.github.com/repos/QuyDuong106/OPENCV_Python/forks",
      "keys_url": "https://api.github.com/repos/QuyDuong106/OPENCV_Python/keys{/key_id}",
      "collaborators_url": "https://api.github.com/repos/QuyDuong106/OPENCV_Python/collaborators{/collaborator}",
      "teams_url": "https://api.github.com/repos/QuyDuong106/OPENCV_Python/teams",
      "hooks_url": "https://api.github.com/repos/QuyDuong106/OPENCV_Python/hooks",
      "issue_events_url": "https://api.github.com/repos/QuyDuong106/OPENCV_Python/issues/events{/number}",
      "events_url": "https://api.github.com/repos/QuyDuong106/OPENCV_Python/events",
      "assignees_url": "https://api.github.com/repos/QuyDuong106/OPENCV_Python/assignees{/user}",
      "branches_url": "https://api.github.com/repos/QuyDuong106/OPENCV_Python/branches{/branch}",
      "tags_url": "https://api.github.com/repos/QuyDuong106/OPENCV_Python/tags",
      "blobs_url": "https://api.github.com/repos/QuyDuong106/OPENCV_Python/git/blobs{/sha}",
      "git_tags_url": "https://api.github.com/repos/QuyDuong106/OPENCV_Python/git/tags{/sha}",
      "git_refs_url": "https://api.github.com/repos/QuyDuong106/OPENCV_Python/git/refs{/sha}",
      "trees_url": "https://api.github.com/repos/QuyDuong106/OPENCV_Python/git/trees{/sha}",
      "statuses_url": "https://api.github.com/repos/QuyDuong106/OPENCV_Python/statuses/{sha}",
      "languages_url": "https://api.github.com/repos/QuyDuong106/OPENCV_Python/languages",
      "stargazers_url": "https://api.github.com/repos/QuyDuong106/OPENCV_Python/stargazers",
      "contributors_url": "https://api.github.com/repos/QuyDuong106/OPENCV_Python/contributors",
      "subscribers_url": "https://api.github.com/repos/QuyDuong106/OPENCV_Python/subscribers",
      "subscription_url": "https://api.github.com/repos/QuyDuong106/OPENCV_Python/subscription",
      "commits_url": "https://api.github.com/repos/QuyDuong106/OPENCV_Python/commits{/sha}",
      "git_commits_url": "https://api.github.com/repos/QuyDuong106/OPENCV_Python/git/commits{/sha}",
      "comments_url": "https://api.github.com/repos/QuyDuong106/OPENCV_Python/comments{/number}",
      "issue_comment_url": "https://api.github.com/repos/QuyDuong106/OPENCV_Python/issues/comments{/number}",
      "contents_url": "https://api.github.com/repos/QuyDuong106/OPENCV_Python/contents/{+path}",
      "compare_url": "https://api.github.com/repos/QuyDuong106/OPENCV_Python/compare/{base}...{head}",
      "merges_url": "https://api.github.com/repos/QuyDuong106/OPENCV_Python/merges",
      "archive_url": "https://api.github.com/repos/QuyDuong106/OPENCV_Python/{archive_format}{/ref}",
      "downloads_url": "https://api.github.com/repos/QuyDuong106/OPENCV_Python/downloads",
      "issues_url": "https://api.github.com/repos/QuyDuong106/OPENCV_Python/issues{/number}",
      "pulls_url": "https://api.github.com/repos/QuyDuong106/OPENCV_Python/pulls{/number}",
      "milestones_url": "https://api.github.com/repos/QuyDuong106/OPENCV_Python/milestones{/number}",
      "notifications_url": "https://api.github.com/repos/QuyDuong106/OPENCV_Python/notifications{?since,all,participating}",
      "labels_url": "https://api.github.com/repos/QuyDuong106/OPENCV_Python/labels{/name}",
      "releases_url": "https://api.github.com/repos/QuyDuong106/OPENCV_Python/releases{/id}",
      "deployments_url": "https://api.github.com/repos/QuyDuong106/OPENCV_Python/deployments",
      "created_at": "2023-08-28T08:05:58Z",
      "updated_at": "2023-08-28T08:07:12Z",
      "pushed_at": "2023-08-31T09:51:27Z",
      "git_url": "git://github.com/QuyDuong106/OPENCV_Python.git",
      "ssh_url": "git@github.com:QuyDuong106/OPENCV_Python.git",
      "clone_url": "https://github.com/QuyDuong106/OPENCV_Python.git",
      "svn_url": "https://github.com/QuyDuong106/OPENCV_Python",
      "homepage": null,
      "size": 49688,
      "stargazers_count": 0,
      "watchers_count": 0,
      "language": "Jupyter Notebook",
      "has_issues": true,
      "has_projects": true,
      "has_downloads": true,
      "has_wiki": true,
      "has_pages": false,
      "has_discussions": false,
      "forks_count": 0,
      "mirror_url": null,
      "archived": false,
      "disabled": false,
      "open_issues_count": 0,
      "license": null,
      "allow_forking": true,
      "is_template": false,
      "web_commit_signoff_required": false,
      "topics": [

      ],
      "visibility": "public",
      "forks": 0,
      "open_issues": 0,
      "watchers": 0,
      "default_branch": "main",
      "score": 1.0
    }
  ]
}
```

3. What Languages are in your Favorite Repo?
```
C:\Users\D U O N G\advanced-git-exercises>curl "https://api.github.com/repos/nodejs/node/languages"
{
  "JavaScript": 13307859,
  "C++": 4766866,
  "Python": 2353499,
  "C": 615402,
  "HTML": 163390,
  "Shell": 99227,
  "Makefile": 53723,
  "Batchfile": 41870,
  "Emacs Lisp": 14363,
  "Perl": 11715,
  "R": 8037,
  "TypeScript": 702,
  "Assembly": 157,
  "Dockerfile": 33
}```