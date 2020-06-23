---
title: "Why Use Elixir For Web Development"
date: 2020-06-23T07:12:23-06:00
tags: [overview]
---

Web development is constantly evolving. Many lessons have been learned through this constant change. Fads have come and gone. Modern web development, and its needs, are now well defined.

The Elixir programming language was born in the middle of the strife. Many web languages exist. Elixir challenges their effectiveness and advantages. The Elixir language addresses the demands of modern web development.

## Needs of Modern Web Development

Walk into any web development shop and you quickly learn their needs — web systems need to be: fast, simple, scalable, maintainable, fault tolerant, and promote programmer happiness. Languages and their frameworks prioritize these needs differently. At times, they are an afterthought. Striking the right balance between them all is challenging. Doing so results in a piece of technology that is fun to use and gets the job done well. Everyone, and everything, should win. Elixir’s origin story helps illustrate how it meets these needs.

## Brief History of Elixir

The needs of web development, already mentioned above, can be broken down into two categories: _technical_ and _programmer-focused_ needs. The technical needs of a modern web development are driven by the web system itself. Systems need to be fast, scalable, and fault tolerant. The programmer-focused needs are driven by programmer needs. Programmers need code that is simple, maintainable, and a language that promotes their happiness. The history of Elixir, and its relation to Erlang, address these category of needs.

Elixir is a functional language made in 2012. José Valim, the creator, was a core member of the Ruby on Rails framework. [José loved the Rails framework](https://weblog.rubyonrails.org/2015/10/22/matthewd-core-josevalim-alum/) and Ruby language emphasis on programmer happiness. He recognized the language’s weaknesses in scalability and slowness. He decided to build a new language to bridge the gap. He chose to build off the success of the Erlang language. [Erlang is known as a concurrent and productive coding language](https://www.erlang-solutions.com/blog/which-companies-are-using-erlang-and-why-mytopdogstatus.html). He designed Elixir to be compatible with the Erlang (aka Beam) VM. As such, Elixir benefits from the existing Erlang ecosystem and battle-tested solutions.

Since Elixir is based on Erlang, the technical needs are addressed. Erlang is a language of choice for building fault fast, tolerant, and scalable systems. The language syntax though is a bit esoteric and dated, by some opinions. Elixir addresses the programmer-focused needs. The syntax and design decisions of the language make the code simple, maintainable, and fun to write in. Elixir, due to its syntax and being built on the Erlang VM addresses the needs of modern web development.

## Elixir and Erlang Address The Needs

Elixir, and its underlying technology Erlang, are designed to meet the needs of modern web development. The following section explain features of Elixir and Erlang that meet the demands of the highlighted needs.

### Fast

Several [benchmarks](https://stressgrid.com/blog/benchmarking_go_vs_node_vs_elixir/) show the speed of Elixir. Web requests can be completed in microseconds. If written correctly, by taking advantage of Elixir’s concurrency model, huge workloads can be handled with ease. Writing concurrent code can be scary, but the [OTP](https://elixirschool.com/en/lessons/advanced/otp-concurrency/) patterns provides a good set of recommendations to follow to properly use Elixir’s concurrency features. Performing work concurrently enables a computer’s full resources to be utilized.

### Scalable

Several [benchmarks](https://stressgrid.com/blog/benchmarking_go_vs_node_vs_elixir/) show the scalability of Elixir. It’s able to process tens of thousands of web connections simultaneously. The concurrency model of Elixir makes this possible. Each connection is handled in an Erlang process independent of all others (Erlang processes differ from. For more details, read [Concurrent Programming](http://erlang.org/doc/getting_started/conc_prog.html).) A single Erlang VM can handle _many_ Erlang processes since they are lightweight.

### Simple

Elixir code is pleasant to look at. It’s syntax makes the code easy to read and write. Elixir is an expressive language without becoming understandable. However, many of the language features that make the syntax simple are not found in object-oriented languages. Much of Elixir’s simplicity is due to its functional features. It takes time for a developer to become familiar with these features. But after embracing features like piping and pattern matching, the code becomes more expressive, simple, and easier to follow.

### Maintainable

Like Elixir’s simplicity, its maintainability rests heavily on its functional features. Elixir uses immutable data structures, encourages writing functions that do not have side effects, and other practices that keep a system maintainable. Knowing that calling a function cannot ever change your local data is freeing. It prevents many bugs that occur due to unintended side effects of calling other code.

### Fault Tolerant

Elixir and Erlang share a motto: let-it-fail. Let-it-fail recognizes that programs run in an imperfect world and so sometimes unexpected events happen. Many programmers try to account for all scenarios using traditional _try-catch blocks_. A better way exists. Elixir and Erlang address the unknown and known scenarios of application failure by encouraging code design that is allows operations to fail. A supervisor process then is in charge of observing for failures and restarting tasks and processes when appropriate so the work can be retried.

Whole books can be written on how fault tolerant applications can be designed. Future posts will cover this topic more in depth later on.

### Promotes Programmer Happiness

Elixir is built by developers who work on production systems daily. They intentionally design the language and tools to be easy to use and understand. The core team listens to the community. Features are added to the language each major/minor release as a result of community requests and needs. Developers lives are made more productive and happy due to the attention the core team gives to the community.

## Conclusion

Elixir is setup for success. The challenging demands of modern web development are well handled by the design decisions of Elixir and the battle-proven technologies provided by Erlang. The technical and programmer-focuses needs discussed here are all adequately addressed.

## Further Reading

* [Elixir Programming: Facts to Know for Better App Development](https://mlsdev.com/blog/elixir-programming-facts-to-know-for-better-app-development) – Covers much of the same material as here. Provides a more in depth analysis to Elixir as a language.
* [Everything you should know about Elixir in 1000 words](https://www.itechart.com/blog/why-use-elixir-web-development-pros-and-cons-itechart-blog/) – Very quick read highlighting the pros and cons of Elixir.

## Updates

* Added the _Elixir and Erlang Address The Needs_ section to explain how each highlighted need is met by Elixir and Erlang.
* Dropped the _Phoenix_ section in favor of covering it more thoroughly in a later post.
