
# Welcome to My Space: Where Life, Love, and Meaning Meet

Hi, I’m [Your Name or “A Heart That Remembers”].

I started this blog not to teach, not to preach — but to **share what I’ve learned, felt, and lived** — so that if you’re walking through grief, confusion, or just the quiet ache of everyday life… you might find a little comfort here.

This is a place for:

- 🌱 **The meaning of life** — not as a philosophy, but as a lived experience.  
- 💰 **Money, work, and investment** — not to make you rich, but to help you feel *free*.  
- 👨‍👩‍👧‍👦 **How to be a good father** — not perfect, but present.  
- 🧒 **Helping kids grow** — with patience, love, and a little grace.  
- 🕘 **Work-life balance** — because you’re not a machine. You’re a human being.  
- ❤️ **Love, family, neighbors** — because joy is found in the small, daily acts of care.

I write from a place of **real life** — not perfection. I’ve grieved. I’ve made mistakes. I’ve learned the hard way. And I want to share those lessons — not to fix you, but to remind you:  
> *You’re not alone. You’re not broken. You’re still growing — and that’s enough.*

This blog is for anyone — whether you’re a parent, a worker, a dreamer, a doubter, or someone just trying to figure out how to live well. No dogma. No pressure. Just honest, gentle, human stories — and practical thoughts that might help you breathe a little easier.

> *“Above all else, guard your heart, for everything you do flows from it.”*  
> — **Proverbs 4:23**
> *(A quiet truth — whether you call it faith, intuition, or simply love — your heart holds your life. Treat it with care.)*

Thank you for being here.  
Let’s walk this path — together.


## Implementation

This website was built using the theme [HugoPlate](https://github.com/zeon-studio/hugoplate).
If you would like to start with this theme, you need to do the following to make it work:

- change 'baseURL' in [hugo.toml](./hugo.toml) to your own website url, such as
  "https://fortune9.github.io/dont-shut-joy-out/" in my case
- to deploy to github pages, go to your github repo, Choose *Settings* > *Pages*, and
  then choose the *Build and deployment* source to *GitHub Actions*. That is it. The
  github action workflow [file](./.github/workflows/main.yml) will take care of the rest,
  which includes building the website and deploy to the pages. If you want to write your
  own workflow, check [this page](https://gohugo.io/host-and-deploy/host-on-github-pages/)
  from Hugo.
- I modified the *Setup Project* in the github action workflow file by adding theme-setup
  to account for any theme changes, such as removing multilingual, etc. This may be optional
  for you.

### To add a new post

```
hugo new posts/your-post-title.md
```

Then edit the newly created markdown file in `content/posts/your-post-title.md`.

### To run the website locally

```
hugo server -D
```

Then open your browser at `http://localhost:1313/`. Here the option `-D` is to include
the draft posts.

### To build the website

```
hugo
```

The generated website will be in the `public` folder.

Since the github action workflow will build the website and deploy to github pages,
you do not need to build the website locally unless you want to check the generated
files.

