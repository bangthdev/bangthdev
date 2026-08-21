<h1>Hi, I'm Bang 👋</h1>

<p>
  I'm a <b>fullstack developer</b> from 🇻🇳 <b>Hanoi, Vietnam</b>, working mostly in
  <b>Go</b> and <b>TypeScript</b>.<br/>
  The part of the job I enjoy is the part nobody demos: making sure people get charged the right
  amount, making sure a job that failed halfway doesn't quietly do everything twice, and finding out
  why a page is slow only for real users.
</p>

<p>
  <img alt="Open to work" src="https://img.shields.io/badge/Open%20to%20work-Backend%20%2F%20Fullstack-2ea44f?style=for-the-badge" />
  <a href="mailto:bangth.dev@gmail.com"><img alt="Email" src="https://img.shields.io/badge/Email-bangth.dev%40gmail.com-D14836?style=for-the-badge&logo=gmail&logoColor=white" /></a>
</p>

<h3>Things I build with</h3>

<p>
  <img
    src="https://skillicons.dev/icons?i=go,ts,nodejs,react,nextjs,postgres,mongodb,redis,prisma,docker,githubactions,linux&perline=6"
    alt="Go, TypeScript, Node.js, React, Next.js, PostgreSQL, MongoDB, Redis, Prisma, Docker, GitHub Actions, Linux"
  />
</p>

<h3>🚀 What I've built</h3>

<table>
  <thead align="left">
    <tr>
      <td><b>Project</b></td>
      <td><b>What it is</b></td>
      <td><b>Built with</b></td>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><a href="https://github.com/bangthdev/Happyfeeling"><b>Happyfeeling</b></a></td>
      <td>A bot that reviews your pull requests for you and comments on the lines that need attention</td>
      <td>TypeScript · Postgres · Redis · Docker</td>
    </tr>
    <tr>
      <td><a href="https://github.com/bangthdev/taphoa-management"><b>taphoa-management</b></a></td>
      <td>Shop software for a grocery store — till, stock, customer debt, and an assistant you can ask questions</td>
      <td>Go · PostgreSQL · React</td>
    </tr>
    <tr>
      <td><a href="https://github.com/DuyDao2311/room_management"><b>room_management</b></a></td>
      <td>Rental and booking site, my graduation project with three classmates (<a href="https://room-management-pearl.vercel.app">live demo</a>)</td>
      <td>Node.js · MongoDB · React</td>
    </tr>
  </tbody>
</table>

<details>
<summary><b>What I did on each one</b></summary>

<br/>

**Happyfeeling** — I own the repository and set up how the project was structured. I built the part
that talks to GitHub, and shared the review pipeline with my teammate.

The problem worth telling: the AI kept leaving its comments on the wrong lines, because it reports
line numbers from memory and gets them slightly wrong. We stopped using its numbers and made it
quote the exact line instead, then searched the real changes for that quote. If the quote is
ambiguous, we drop the comment rather than guess.

I also reviewed my teammate's pull requests and caught a few things before they merged — a database
update that silently never refreshed its timestamp, and a secrets file that was being copied into
the published Docker image.

**taphoa-management** — built on my own, for a shop that actually uses it. Go backend, PostgreSQL,
and a deploy script that sets the server up to run in the background on a fresh Ubuntu machine.

The interesting part is the stock: goods arrive in batches with different expiry dates, so a sale
has to take from the batch expiring soonest. Otherwise stock quietly rots on the shelf while newer
stock gets sold. There's also a job that emails the owner about anything close to expiring, and an
assistant that answers questions about stock and can read a photo of an invoice.

**room_management** — a graduation project with three classmates. I built the services side of it
end to end: the data models, the API, and the admin screens for managing services and their
bookings. I also wrote the email notifications, the forgot-password flow, and the tests covering all
of it.

</details>

<h3>🏢 Where I've worked</h3>

<b>Backend / Fullstack Intern</b> — a workflow automation and blockchain platform · Jan–Jun 2026

Most of what I learned there lives in a private company repository, so here's what it was:

- **Reviewing a large payment change.** I found a bug that charged people on Stripe but never
  actually upgraded their plan, and a missing safeguard that let the same charge go through twice.
- **Trying to break the billing system on purpose.** The tests I designed turned up a downgrade that
  took effect immediately instead of at the end of the billing period — which quietly paused
  automations people were still using. We fixed it by holding the change until the period ended.
- **Chasing a slow page that was only slow in production.** It turned out not to be the backend at
  all: the browser was refetching data it already had, because a caching setting was missing.
  Afterwards, loading the same page again makes no network request at all.
- **Fixing a query that lost people money.** Upgrading a plan wiped a customer's free credits and
  counted them as if they had been spent. I fixed the calculation and the balances came back.
- **Laying out a canvas.** The editor arranged connected blocks fine, but fell apart when the
  diagram had separate, unconnected groups. I rewrote that part so every group gets placed properly.

<h3>🎓 Education</h3>

**B.Eng. Information Technology** — Posts and Telecommunications Institute of Technology (PTIT),
2021–2026. Degree conferred Oct 2026.

Vietnamese (native) · Chinese (HSK 3–4) · English (Aptis ESOL B1)

<h3>📈 What I'm doing now</h3>

Solving algorithm problems in Go every weekday, and reading real codebases to get better at the
thing I'm weakest at — understanding unfamiliar code on my own.

<h3>📫 Say hello</h3>

<p>
  <a href="mailto:bangth.dev@gmail.com"><img alt="Gmail" src="https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white" /></a>
  <a href="https://github.com/bangthdev"><img alt="GitHub" src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white" /></a>
</p>
