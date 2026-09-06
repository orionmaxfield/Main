# Orion Maxfield — site (generation 4: the shade)

Eight files. No build step, no dependencies. Every page is self-contained and previews on its own.

## The idea the whole site runs on

**Seen → Safe → Strong.** The home page and "If you're here" open in *glare* (white, black, honest,
names the pain), drop into *shade* (deep green, dappled, "sit down for a minute"), then open into
the calm *stone* pages where he chooses a path. Faith is hinted, never named. The man under the
tree is never identified. Keep it that way.

## Pages

| File | Job |
|---|---|
| `index.html` | Glare hero → shade → four paths → about → email |
| `if-youre-here.html` | The doorway. The one page that says the rough words out loud (search + recognition). Links to Start Here. |
| `start-here.html` | The first kind thing: three true things, out loud, one more a day for a week. Free, no email. The seven-day sheet is the email ask. |
| `writing.html` | Essays sorted into four rooms with anchors: `#late-nights`, `#futility`, `#rules`, `#dating` |
| `writing/not-lazy.html` | First essay |
| `about.html` | The mountain, then who you are, then what this is and isn't |
| `resources.html` | Tools, AI-as-a-tool-not-a-therapist, crisis lines, ARP |
| `contact.html` | Form + email |

## Before you go live — replace these

| Where | What |
|---|---|
| `index.html`, `about.html` | Add your photo to the repo as `portrait.jpg` (exact name). Until then the space simply stays empty. |
| `index.html`, `writing.html`, `start-here.html`, `writing/not-lazy.html` | `PASTE_YOUR_PROVIDER_FORM_URL_HERE` — your email provider's form URL (Buttondown / Kit / MailerLite) |
| `contact.html` | `PASTE_YOUR_FORMSPREE_ENDPOINT_HERE` and `PASTE_YOUR_EMAIL_HERE` |
| `writing/not-lazy.html`, `writing.html` | The word `Draft` → a real date when you publish |
| Email provider | The Start Here signup promises **the seven-day sheet**. Make a one-page PDF and set it as the provider's welcome email before the form goes live. |
| `writing.html` | Three "In progress" titles are placeholders for the first piece in each room. Write them or delete the `<li>`. |

**Supervisor review before publishing.** The doorway page names pornography and scrupulosity
directly, and the About page tells the mountain story. Both are written to stay universal and
non-confessional, but Utah pre-licensure advertising rules are your supervisor's call.

## Uploading (replacing the old files on GitHub)

The file names changed. In the repo, delete the old `index.html`, `about.html`, `writing.html`,
`resources.html`, `contact.html`, `writing/not-lazy.html`, then add all eight files from this
folder. Or connect Claude Code to the repo and ask it to replace everything with this folder.

## Adding a new piece

1. Copy `writing/not-lazy.html`, rename it (lowercase, hyphens). Change the room link at the top,
   the title, byline, and text.
2. In `writing.html`, copy the `<li>` block under the matching room and point it at the new file.
   Newest at the top. Delete the "In progress" placeholder when a real piece replaces it.

## Design tokens (keep them)

- Glare: `#FFFFFF` / `#000000` (dark mode: inverted)
- Shade: `#1B332C` background, `#EEF3EC` text, dappled with three radial gradients
- Stone (default pages): `#F4F5F1` / `#12201B`, link `#225744`; dark mode `#131916` / `#EEF1EC`
- Type: Literata (serif, everything) + Public Sans (nav, buttons, small labels)
- Body 19px, line-height 1.65, measure 38rem

The rule from the design: glare and shade only appear where a man is arriving — the home page,
the doorway, the top of Start Here, and the signup after an essay. Everything else is stone.
