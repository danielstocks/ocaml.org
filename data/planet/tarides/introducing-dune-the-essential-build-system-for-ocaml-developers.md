---
title: 'Introducing Dune: The Essential Build System for OCaml Developers'
description: "One of the first tools you'll encounter when adopting OCaml is Dune,
  OCaml's official build system. Understanding what Dune is and how it\u2026"
url: https://tarides.com/blog/2024-09-26-introducing-dune-the-essential-build-system-for-ocaml-developers
date: 2024-09-26T00:00:00-00:00
preview_image: https://tarides.com/static/a56b0f2b093434d01f3a8fe23d92e45f/29df2/intro_dune.jpg
authors:
- Tarides
source:
---

<p>One of the first tools you'll encounter when adopting OCaml is Dune, OCaml's official build system. Understanding what Dune is and how it serves you is key to crafting everything from a small project to maintaining large-scale codebases. So let's dive in! Learn how Dune makes development easier and serves as a gateway to the greater OCaml Platform.</p>
<p>For a quick introduction to OCaml, check out the <a href="https://ocaml.org/docs/installing-ocaml">tutorials on OCaml.org</a>.</p>
<h3 style="position:relative;"><a href="https://tarides.com/feed.xml#what-is-dune" aria-label="what is dune permalink" class="anchor before"><svg aria-hidden="true" focusable="false" height="16" version="1.1" viewbox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>What is Dune?</h3>
<p>Dune is much more than a simple build tool. It automatically compiles your OCaml code, manages its dependencies, and generates the final executable or library. It's also a well-maintained, highly-optimised platform that streamlines your development process. Spend more time writing code and less on struggling with complex build rules.</p>
<h3 style="position:relative;"><a href="https://tarides.com/feed.xml#advantages-of-dune" aria-label="advantages of dune permalink" class="anchor before"><svg aria-hidden="true" focusable="false" height="16" version="1.1" viewbox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Advantages of Dune</h3>
<h4 style="position:relative;"><a href="https://tarides.com/feed.xml#1-consistency-across-projects" aria-label="1 consistency across projects permalink" class="anchor before"><svg aria-hidden="true" focusable="false" height="16" version="1.1" viewbox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>1. <strong>Consistency Across Projects</strong></h4>
<p>With Dune, you can be sure that the build processes are consistent, no matter how many different projects you are managing. This is very helpful when collaborating with other developers or when maintaining multiple projects. Once you work with Dune on one project, it's easier to work on the next, even if it has a totally different codebase, because Dune standardises how things are done.</p>
<h4 style="position:relative;"><a href="https://tarides.com/feed.xml#2-integration-with-the-ocaml-platform" aria-label="2 integration with the ocaml platform permalink" class="anchor before"><svg aria-hidden="true" focusable="false" height="16" version="1.1" viewbox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>2. <strong>Integration With the OCaml Platform</strong></h4>
<p>Dune lives on the cutting edge of the OCaml Platform (a set of tools and libraries) and forms a solid foundation for your development environment. Dune automatically plays nicely with other tools such as opam (an OCaml package manager) and helps you manage dependencies, run tests, and set up project documentation.</p>
<h4 style="position:relative;"><a href="https://tarides.com/feed.xml#3-performance-optimisation" aria-label="3 performance optimisation permalink" class="anchor before"><svg aria-hidden="true" focusable="false" height="16" version="1.1" viewbox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>3. <strong>Performance Optimisation</strong></h4>
<p>Dune is fast and efficient. It tracks dependencies and rebuilds only when necessary, so your development processes will be more responsive. This performance optimisation benefits the developer, regardless of project size. Although for big projects, it especially makes a difference because it significantly reduces the build time.</p>
<p>Dune also supports other languages and tools within the same project. This flexibility makes it easy to incorporate C stubs, inline assembly, or even JavaScript (via js_of_ocaml and <a href="https://melange.re/v2.1.0/">Melange</a>) into your OCaml projects without needing to change your build system.</p>
<h3 style="position:relative;"><a href="https://tarides.com/feed.xml#a-well-maintained-and-evolving-tool" aria-label="a well maintained and evolving tool permalink" class="anchor before"><svg aria-hidden="true" focusable="false" height="16" version="1.1" viewbox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>A Well-Maintained and Evolving Tool</h3>
<p>The Dune team listens to community needs and regularly releases updates for performance, features, and bug fixes. This keeps Dune current with OCaml's development, giving engineers a coherent and state-of-the-art tool that evolves with the language and ecosystem.</p>
<p>Soon, Dune will also provide package managing functionality, so you can choose whether to use Dune or opam. It's currently in beta testing, so watch this blog for an announcement of the upcoming release!</p>
<h3 style="position:relative;"><a href="https://tarides.com/feed.xml#getting-started-with-dune" aria-label="getting started with dune permalink" class="anchor before"><svg aria-hidden="true" focusable="false" height="16" version="1.1" viewbox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Getting Started With Dune</h3>
<p>It is very easy to install Dune using opam:</p>
<div class="gatsby-highlight" data-language="sh"><pre class="language-sh"><code class="language-sh">opam <span class="token function">install</span> dune</code></pre></div>
<p>Now make a new OCaml project by running:</p>
<div class="gatsby-highlight" data-language="sh"><pre class="language-sh"><code class="language-sh">dune init project my_project</code></pre></div>
<p>This creates a minimal project structure with sensible defaults, so you can get to coding right away. When ready, compile your project using <code>dune build</code> and run it using <code>dune exec ./my_project</code>.</p>
<h3 style="position:relative;"><a href="https://tarides.com/feed.xml#conclusion" aria-label="conclusion permalink" class="anchor before"><svg aria-hidden="true" focusable="false" height="16" version="1.1" viewbox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Conclusion</h3>
<p>Dune simplifies the development process, ensures uniformity, and is deeply integrated with the entire OCaml Platform. If you set up Dune from the very beginning, it will let you focus on creating great software, the most important thing.</p>
<p>As you learn more about OCaml, you'll appreciate the power, flexibility, and great community behind Dune and OCaml as a whole. For both small personal projects and collaborations on big applications, Dune is a tool you can rely on from start to finish.</p>
<blockquote>
<p>At Tarides, open source is at our core. The company was founded with a key mission of serving the OCaml community and <a href="https://github.com/sponsors/tarides">improving the OCaml language</a>. We are keen to work with industry partners and individual developers in pursuit of improving OCaml's performance and feature set, and we want you to be an active participant in the OCaml community. Learn about the language, try its tools, and contribute to its ongoing evolution.</p>
</blockquote>
<blockquote>
<p>Tarides also offers commercial services related to OCaml. Whether it is training, support or tailored development, we can assist industrial users in exploiting OCaml 5 to its full potential. Please do not hesitate to <a href="https://tarides.com/contact/">contact us</a> to discuss your needs.</p>
</blockquote>
<blockquote>
<p>Follow us on <a href="https://twitter.com/tarides_">Twitter</a> and <a href="https://www.linkedin.com/company/tarides/">LinkedIn</a> to ensure you never miss a post We've also created new accounts on <a href="https://mastodon.social/@tarides">Mastodon</a> and <a href="https://www.threads.net/@taridesltd">Threads</a>, if you prefer. Be sure to join the OCaml discussion on <a href="https://discuss.ocaml.org/">Discuss</a>!</p>
</blockquote>