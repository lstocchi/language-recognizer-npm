# API Library for language/framework recognition

A NPM package providing helpers for recognize languages/frameworks used in a project.

The package is based on the `languages` file created by Guthub for its [Linguist project](https://github.com/github/linguist).

It recognizes all programming languages as GitHub Linguist and several additional frameworks:

- Java Quarkus
- Java SpringBoot
- Java OpenLiberty
- Java Micronaut
- Python Django

## Examples

```
import * as recognizer from 'language-recognizer';

.....

const languages = await recognizer.detectLanguages('my_project_folder');

.....

```

### Outputs 

Quarkus project output example

```
[
  { name: 'java', builder: 'maven', frameworks: [ 'quarkus' ] },
  { name: 'gcc machine description' }
]
```

SpringBoot project output example

```
[
  { name: 'java', builder: 'maven', frameworks: [ 'springboot' ] },
  { name: 'plsql' },
  { name: 'plpgsql' },
  { name: 'sqlpl' },
  { name: 'tsql' },
  { name: 'javascript' },
  { name: 'batchfile' },
  { name: 'gcc machine description' }
]
```

Django project output example

```
[
  { name: 'python', frameworks: [ 'django' ] },
  { name: 'gcc machine description' },
  { name: 'shell' }
]
```

## Contributing

This is an open source project open to anyone. This project welcomes contributions and suggestions!

## Feedback & Questions

If you discover an issue please file a bug in [GitHub issues](https://github.com/lstocchi/language-recognizer-npm/issues) and we will fix it as soon as possible.

## License

MIT, See [LICENSE](https://github.com/lstocchi/language-recognizer-npm/blob/master/LICENSE.md) for more information.