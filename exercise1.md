A small developer team is working on a backend application written in Go (a language/environment I'm not familiar with). Compared to JS or Java, Go has a very small ecosystem and selection of used tools does not pose a problem.

The usual setup for Go application development seems to be self-hosted environment using mostly built-in tools of the Go language package. For linting and code verification, there are several open source tools available, for example built-in "go vet" and golint.

The Go language also includes unit testing functionality. There's not much choice but the good thing is that no matter which CI environment, that testing method will be supported.

Building executables is again based on Go standard tools. Automation tools for going through linting, testing, building and deploying exist, starting from the standard UNIX make but also more advanced tools such as Gödel are available.

A complete self-hosted CI for Go could be e.g. GoCD, Gitlab or Buddy.

Cloud CI do generally have good Go support, for example CircleCI, Semaphore.

A cloud-based CI environment makes sense in this case because setting up a self-hosted environment, however small, takes some effort. A cloud-based solution provides better support and is available immediately. Setting up the CI pipeline may be quicker in a cloud-based environment, as well. The downside is cost.
