# httpbin(1): HTTP Request & Response Service

This is a fork of the original httpbin project, which is located at https://github.com/postmanlabs/httpbin

Why fork?  we were unable to get ahold of the folks at postmanlabs to maintain the original project, and httpbin is used for other packages within the python ecosystem, such as [pytest-httpbin](https://pypi.org/project/pytest-httpbin/) which is in turn used by packages such as [requests](https://github.com/psf/requests/blob/main/requirements-dev.txt#L4) so we have forked this package.  That means that httpbin.org is not actually backed by this repo, but the [httpbin package](https://pypi.org/project/httpbin/) is.  Confusing right?  Know anyone at postmanlabs?  [get in touch](mailto:me@kevinmccarthy.org).

httpbin is a [Kenneth Reitz](http://kennethreitz.org/bitcoin) Project.
![ice cream](http://farm1.staticflickr.com/572/32514669683_4daf2ab7bc_k_d.jpg)

Run locally:
```sh
docker pull kennethreitz/httpbin
docker run -p 80:80 kennethreitz/httpbin
```

Some enviroments do not allow to bind to a privileged port. To run it on a
different port instead of port 80, set the environment variables as follows:

```sh
docker run -e HTTPIN_PORT=8000 -p 8000:8000 kennethreitz/httpbin
```

See http://httpbin.org for more information.

## Officially Deployed (but out of date) at:

- http://httpbin.org
- https://httpbin.org
- https://hub.docker.com/r/kennethreitz/httpbin/


## SEE ALSO

- http://requestb.in
- http://python-requests.org
- https://grpcb.in/

