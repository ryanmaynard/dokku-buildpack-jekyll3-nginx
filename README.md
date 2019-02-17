This is a dokku buildpack for installing Jekyll 3. It uses `Ruby 2.6.1` and `nginx 1.5.7`

Tested with:
- `dokku 0.13.4` and `jekyll-3.6.2` on `Ubuntu 18.04.2`

### Usage

Just add a `.buildpacks` file in the root of your Jekyll project containing:

```
https://github.com/heroku/heroku-buildpack-nginx.git
https://github.com/ryanmaynard/dokku-buildpack-jekyll3-nginx.git
```

(Delete any previous `.env` file that contain `export BUILDPACK_URL=...`)

### Other

For Jekyll 2.x, use [inket/dokku-buildpack-jekyll-nginx](https://github.com/inket/dokku-buildpack-jekyll-nginx)

### Credit

Fork tree:


- [ryanmaynard/dokku-buildpack-jekyll3-nginx](https://github.com/ryanmaynard/dokku-buildpack-jekyll3-nginx)
	- [inket/dokku-buildpack-jekyll-nginx](https://github.com/inket/dokku-buildpack-jekyll-nginx)

		- [shsteven/dokku-buildpack-jekyll-nginx](https://github.com/shsteven/dokku-buildpack-jekyll-nginx)

			- [nbudin/heroku-buildpack-jekyll-nginx](https://github.com/nbudin/heroku-buildpack-jekyll-nginx)

				- [mchung/heroku-buildpack-nginx](https://github.com/mchung/heroku-buildpack-nginx)
