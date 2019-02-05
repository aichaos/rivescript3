# RiveScript 3

```
! version = 3
```

This is an **in-development** new version of the
[RiveScript](https://www.rivescript.com/) chatbot scripting language.

RiveScript is a simple text-based language for creating chatbots that respond to
pre-programmed patterns with clever responses. Version 2 of the language was
implemented in five different programming languages by its author and supported
and maintained with the help of contributors on GitHub: Perl, Java, Python,
JavaScript and Go. Across these five languages RiveScript has amassed hundreds
of users and spawned a few startups in bot hosting services.

RiveScript 3 will be **backwards compatible** in that the RS3 interpreter will
be able to read and use your existing RiveScript 2 code just fine while
supporting new tags and syntax in new source files.

## Quick Facts

* I'm only going to program RiveScript 3 in one programming language, not five.
* That language is going to be **Go**.
* I will make it backwards compatible to RiveScript 2 so that you can mix and
  match files written in either dialect in the same chatbot.
    * Designated by that header, `! version = 3`
    * Will use the [rivescript-go](https://github.com/aichaos/rivescript-go)
      library to understand RiveScript 2 syntax, and translating it into the
      new engine will be a first-class feature to be kept working.
* I'll explore ways to create tight bindings to the existing programming
  languages that have a lot of existing RiveScript users:
  * **JavaScript:** via GopherJS and WebAssembly, which I've experimented with
    before in Go at [rsgb](https://github.com/aichaos/rsgb).
  * **Python:** via CPython API for native modules.
  * **Other:** Go makes for really good web servers, so RiveScript 3 can
    include a built-in RESTful API over good old HTTP.
* All development of RS3, including its language specification, will be kept
  at https://github.com/aichaos/rivescript3 _at least until_ the stable release
  of the project.

## License

MIT. Noah Petherbridge &copy; 2019.
