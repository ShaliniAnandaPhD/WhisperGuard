# 📘 BUILD FOR HER · Team guide to GitHub

Never used GitHub? You're in the right place. This takes about 10 minutes, and every teammate can do it from a browser.

**GitHub in one sentence:** it's a shared online folder for your project, where every change is saved with a note so nothing gets lost. Your team's folder is called a **repository** (or "repo"), and saving a change is called a **commit**.

---

## Step 1 · Make your team's copy (one person, 2 min)

Usually the technical builder does this.

1. Sign in to GitHub. No account yet? Make a free one at [github.com/signup](https://github.com/signup).
2. Open the starter template: [github.com/buildforher-sf/build-for-her-starter](https://github.com/buildforher-sf/build-for-her-starter)
3. Click the green **Use this template** button → **Create a new repository**.
4. **Owner:** your own account. **Repository name:** your project's name, like `safe-route`.
5. Choose **Public** (easiest for judging), then **Create repository**.

<details>
<summary>Want to keep your repo private?</summary>

That's okay. Go to **Settings → Collaborators → Add people** and add **`mlyab`** so the judges can see it.

</details>

## Step 2 · Invite your teammates (1 min)

In your new repo: **Settings → Collaborators → Add people**, then type each teammate's GitHub username. They'll get an invite by email and on GitHub; they need to accept it.

Everyone on the team is a full builder, so everyone should be able to edit.

## Step 3 · Fill in the README (whole team)

The README is your project's front page, and it's the first thing judges read.

1. Click **README.md**, then the ✏️ pencil icon (top right).
2. Replace every ✏️ with your own words. The grey `<!-- notes -->` are tips that only show up in edit mode; you can leave them.
3. Click **Preview** to check how it looks.
4. Click **Commit changes…** → **Commit changes**. That's "save".

**Tip:** if two people edit the same file at the same time, one can overwrite the other. Take turns, or draft together in a shared doc and paste it in once.

## Step 4 · Add your screenshot and deck

1. Open the **docs** folder → **Add file → Upload files**.
2. Drag in your Maritime dashboard screenshot, named exactly **`maritime-dashboard.png`**. It replaces the placeholder and shows up in your README automatically.
3. Optional: drag in your deck as `pitch-deck.pdf`.
4. Click **Commit changes**.

## Step 5 · Add your code

**On your laptop** (technical builders):

```bash
git clone https://github.com/YOUR-USERNAME/YOUR-REPO.git
cd YOUR-REPO
# ...build things...
git add .
git commit -m "Add check-in agent"
git push
```

Push often (every hour is great). It's your backup if a laptop dies, and your history shows the judges you built it today.

**No terminal?** Use **Add file → Upload files** or **Add file → Create new file** in the browser.

**Deploying your own app to Maritime?** Your repo needs a `Dockerfile`. Then:

```bash
maritime create my-app --repo https://github.com/YOUR-USERNAME/YOUR-REPO --public --port 3000
```

Full docs: [maritime.sh/docs](https://maritime.sh/docs)

---

## 🔐 Keep your keys secret

API keys work like passwords. A key pushed to a public repo can be found by bots within minutes.

- Put keys in a file called `.env` on your laptop. This template already tells git to ignore `.env`, so it never gets uploaded. Use `.env.example` as your guide.
- On Maritime, add keys with `maritime env set my-agent KEY=value --reload`, or in the agent's **Settings** tab.
- Pushed a key by accident? **Revoke it right away** on the provider's website and make a new one. Deleting the file isn't enough, because GitHub keeps the history.

## 👥 Who does what (a suggestion)

| Role | Owns |
| --- | --- |
| Technical builder | The code and Maritime · README sections 4, 6, 7 |
| Product or subject-matter expert | Problem, user and responsibility · sections 1, 2, 10 |
| Design | Deck, screenshots, user journey · section 3 |
| Everyone | Demo video, data, next steps, ownership · sections 5, 8, 9, 11 |

## ✅ Before you submit

This mirrors the submission form, so you can check it off as you go:

- [ ] Team name, members, track, and the technical builder's name
- [ ] Problem statement: 2–3 sentences, citing at least one fact or source
- [ ] Maritime agent/instance name, dashboard screenshot, and one sentence on its role
- [ ] GitHub repo link
- [ ] README complete: what it does, how to run it, tools and AI models, libraries/APIs, data sources, pre-existing work
- [ ] Pitch deck: up to 5 slides (PDF or link)
- [ ] Backup demo video: 60–90 seconds
- [ ] Responsibility note: 2–3 sentences for your track

**The judge test (30 seconds):**

1. Open your repo link in a private/incognito browser window. If you see a 404 page, your repo is private: make it public, or add `mlyab` as a collaborator.
2. Search your README for ✏️. If you find one, you're not done yet.

**Submit here:** [submission form](https://stupendous-umbrella-349.notion.site/BUILD-FOR-HER-Attendee-Hub-3f31555b8fe681e489dfdc285ae7448e?source=copy_link) · **Times, rules and help:** [Attendee Hub](https://stupendous-umbrella-349.notion.site/BUILD-FOR-HER-Attendee-Hub-3f31555b8fe681e489dfdc285ae7448e?source=copy_link) · [Discord](https://stupendous-umbrella-349.notion.site/BUILD-FOR-HER-Attendee-Hub-3f31555b8fe681e489dfdc285ae7448e?source=copy_link)

Good luck, builders 💜
