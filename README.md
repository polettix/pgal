# pgal - a gallery generator

[iGal][] is a gallery generator I discovered some time ago. After looking at
it, I decided to reinvent the wheel for good and gave birth to `pgal`.

Now, years after, here it comes, with a slightly renewed code and a packaging
inside a [Docker][] image (thanks to [Alpine Linux][]).

To use the image, define a little helper like this:

```shell
pgal() { docker -itv "$PWD:/mnt" --rm pgal "$@" ;}
```

then call it, e.g.:

```shell
pgal --man
```

This will show your the man page. Then just follow the instructions.


The contents of this repository are licensed according to the Apache
License 2.0 (see file `LICENSE` in the project's root directory):

>  Copyright 2020 by Flavio Poletti
>
>  Licensed under the Apache License, Version 2.0 (the "License");
>  you may not use this file except in compliance with the License.
>  You may obtain a copy of the License at
>
>      http://www.apache.org/licenses/LICENSE-2.0
>
>  Unless required by applicable law or agreed to in writing, software
>  distributed under the License is distributed on an "AS IS" BASIS,
>  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
>  See the License for the specific language governing permissions and
>  limitations under the License.


[iGal]: http://igal.sourceforge.net/
[Docker]: https://www.docker.com/
[Alpine Linux]: https://www.alpinelinux.org/
