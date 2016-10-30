# Amnesty Decoders
In Amnesty's version of PyBossa, multiple projects can be associated with a parent project.

Each child project will have the same URL pattern when loading a new task.

What this means is that project short names like decode-darfur-part-1, decode-darfur-part-2, or decode-darfur-part-3 will still be loaded under one common newtask URL, /project/decode-darfur/newtask, where decode-darfur is the parent project's short name.

We currently manage this with server side URL rewrites. However, we also need to support this in pybossa.js since there is mechanism there to determin the task url based on the project short name instead of the parent project's short name.

The rest of this README is the repository's original README from when it was forked (commit [62b1f7906d0c3901c6e6f58d311805cc0cfd1b48](https://github.com/Scifabric/pybossa.js/commit/62b1f7906d0c3901c6e6f58d311805cc0cfd1b48))

# PyBossa.JS: a JavaScript for PyBossa.

PyBossa.JS is a simple JavaScript library that will allow you to create
a PyBossa project using three methods:

* pybossa.taskLoaded,
* pybossa.presentTask, 
* pybossa.saveTask, and
* pybossa.run('your-slug-project-name')

If you want to learn how to use the library, please, check the demo project and their documentation:

**NOTE**: pybossa.saveTask can have a task object or a task.id. It's up to you.

* [FlickrPerson for PyBossa](https://github.com/PyBossa/app-flickrperson) [[doc]](http://docs.pybossa.com/en/latest/user/create-application-tutorial.html)

If you want more details, check the [documentation](http://pybossajs.rtfd.org).

# Contributing to PyBossa.JS

If you want to contribute to this library, please, read carefully the
[Contribution Guidelines](CONTRIBUTING.md)

# Running Tests

You will need to have [npm](https://www.npmjs.com/) with either Node or io.js.
First time, run:

```
  npm install -g grunt-cli
  npm install
```

And from this point, you can run the tests simply with:

```
  grunt test
```

# Copyright

Copyright 2015 [SciFabric LTD](http://scifabric.com).

# License

GPLv3 (see [COPYING file](COPYING))
