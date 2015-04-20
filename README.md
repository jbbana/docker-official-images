# Official images for docker

### Contributing to the library

- - -
##### Filenames
The filename of a definition file will determine the name of the image repository it creates on the Docker Hub Registry. For example, the `library/hello-world` file will create tags in the `hello-world` repository.

##### Instruction format
```
<docker-tag>: <git-url>@<git-commit-id>

latest: git://github.com/docker-library/hello-world@b7a78b7ccca62cc478919b101f3ab1334899df2b

<docker-tag>: <git-url>@<git-commit-id> <dockerfile-dir>

2.6.17: git://github.com/docker-library/redis@062335e0a8d20cab2041f25dfff2fbaf58544471 2.6
2.6: git://github.com/docker-library/redis@062335e0a8d20cab2041f25dfff2fbaf58544471 2.6
```

##### Creating a new repository

-	Create a new file in the `library/` folder. Its name will be the name of your repository.
-	Add your tag definitions using the appropriate syntax (see above).
-	Add a line similar to the following to the top of the file:

		`# maintainer: Your Name <your@email.com> (@github.name)`

-	Create a pull request adding the file from your forked repository to this one. Please be sure to add details as to what your repository does.

##### Commitment

Proposing a new official image should not be undertaken lightly. We expect and require a commitment to maintain (including and especially timely updates as appropriate) your image.