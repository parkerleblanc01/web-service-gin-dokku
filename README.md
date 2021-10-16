# Simple Go Server using Gin

## Deploying with Dokku using Go
1. Install vendor packages `go mod vendor`
2. Ensure you use a heroku decorator `// +heroku goVersion go1.12`
3. Commit changes `git add . && git commit -m 'deploy commit'`
4. Create the dokku app `dokku apps:create test-go`
5. Add dokku git remote `git remote add dokku dokku@<ip address>:test-go`
6. Push changes to remote `git push dokku master`