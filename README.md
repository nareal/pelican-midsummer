# Pelican-midsummer

This [pelican](http://docs.getpelican.com) theme is a fork of the [pelican-sundown](https://github.com/keningle/pelican-sundown) theme by [Ken Ingle](https://github.com/keningle).

## Configuration

This theme does have a few differences from the original sundown theme.
For example, slightly larger font for content, gravatar image, and
social icons.

Additions such as gravatar are not required, but available.  The
following settings should be added/adjusted in the `pelicanconf.py`:

### Gravatar

You can include a gravatar image in the top left of the template by
adding the following lines to your config:

```python
import urllib, hashlib

# Conf for pulling Gravatar Image
EMAIL = u'youremail@email.com'
DEFAULT_GRV_URL = u'http://www.example.com/default.jpg'
GRV_SIZE = 120

# construct gravatar URL
GRV_URL = "http://www.gravatar.com/avatar/" + hashlib.md5(EMAIL.lower()).hexdigest() + "?"
GRV_URL += urllib.urlencode({'d':DEFAULT_GRV_URL, 's':str(GRV_SIZE)})
``` 

## Who is using pelican-midsummer

* [nelsonareal.net](http://nelsonareal.net)
 
## License (MIT)

The MIT License (MIT)

Copyright (c) 2015, Nelson Areal

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

---

Original pelican-sundown license:

The MIT License (MIT)

Copyright (c) 2013, Ken Ingle

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.
