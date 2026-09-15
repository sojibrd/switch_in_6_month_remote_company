# switch_in_6_month_remote_company

১৮০ দিনের plan: বাংলাদেশে বসে বিদেশি রিমোট কোম্পানিতে ২০টা আবেদন আর অন্তত ৫টা সম্পূর্ণ interview process। মূল বাজার ইউরোপ/যুক্তরাজ্য, offer-এর নিচের সীমা মাসে $১,৭০০। প্রতিদিন একটা করে করার কাজ, শেখার বিজ্ঞান মেনে।

এটা তিনটা বিকল্প plan-এর একটা। একজন একটাই চালায়: [লোকাল](https://github.com/sojibrd/switch_in_6_month_local_company) · **রিমোট** (এটা) · [গ্লোবাল](https://github.com/sojibrd/switch_in_6_month_global_company)। তিনটার কোড হুবহু এক।

**লাইভ:** https://sojibrd.github.io/switch_in_6_month_remote_company/

## Functional Requirement

- **আজ (`/`):** প্রথমবার খুললে শুরুর তারিখ জিজ্ঞেস করে। তারপর ক্যালেন্ডারের আজকের দিন — ক্রম: dip-এর সতর্কতা → জমে থাকা ⚑ মাইলফলক → আজকের ঝালাই → আজকের দিন।
- **Rail:** সব পাতায় বাঁয়ে একটা rail থাকে, মোবাইলে drawer। তাতে ৩টা পাতার লিংক, plan-এর gauge আর ৬টা ব্লক; যে ব্লক খোলা শুধু তার দিনগুলো দেখায়।
- **দিন (`/day/<nnn>/`) · ব্লক (`/block/<slug>/`):** দিনের কাজ আর দিন বা ব্লক শেষের হ্যাঁ/না।
- **ঝালাই (`/review/`):** প্রতিটা 🔁 কাজ টিকের দিন থেকে ১/৩/৭/২১ দিন পরে ফিরে আসে। "মনে ছিল" দিলে পরের ধাপে, "আটকে গেছি" দিলে আজ থেকে আবার ১ দিনে।
- **নিয়ম (`/rules/`):** `docs/00-rules.md` হুবহু।
- **🧠 chip:** চাপলে এক লাইনে দেখায় কেন কাজটা এভাবে, সাথে `learning_to_learn` সাইটের লিংক।

## Non-Functional Requirement

- **সত্যের উৎস `docs/`।** কোডে কোনো ব্লক, দিন বা কাজ হার্ডকোড নেই।
- **ফাইলে তারিখ নেই।** তারিখ = শুরুর তারিখ + (দিন − ১); শুরুর তারিখ ব্রাউজারে। দিন ০০১ = সোমবার ধরে লেখা।
- **"আজ" = ক্যালেন্ডারের তারিখ।** plan পেছায় না। বাদ পড়া সাধারণ কাজ ফেরে না; শুধু ⚑ জমে থাকে।
- **DSA এই সাইটে নয়।** দিন ০০৮–০৭৭ [`dsa_prep_remote_company`](https://sojibrd.github.io/dsa_prep_remote_company/) — এখানে শুধু ঘরটা আর লিংক; ঐ সাইটের তিনটা স্ক্রিন-মহড়া এই plan-এর দিন ০৩৪, ০৬২, ০৭৬-এর শনিবারে।
- **System design-ও এই সাইটে নয়।** দিন ০৭৮–১৩৩ [`system_design_remote_company`](https://sojibrd.github.io/system_design_remote_company/) — DSA শেষে খালি হওয়া সোম–শুক্রের ৩০′-এ, আগে ঝালাই; দিন ১৪০ আর ১৪৭-এ design doc মুখে।
- **Behavioural-ও এই সাইটে নয়।** দিন ০০৬–১৫৪-এর story-র কাজ [`behavioural_interview_remote_company`](https://sojibrd.github.io/behavioural_interview_remote_company/)-এ — হুবহু সরানো, ঐ সাইটের দিন = এই plan-এর দিন − ৫; এখানে ঘর আর লিংক, রোজের ইংরেজি আর mock।
- **Static export → GitHub Pages।** Backend নেই।
- **Progress শুধু `localStorage`-এ,** একমাত্র `app/hooks/useProgress.ts` দিয়ে। **`app/lib/plan.ts` server-only।**
- **তিন plan-এর কোড এক।** পার্থক্য শুধু `app/lib/site.ts`, `next.config.ts`-এর basePath আর `docs/`। কোড বদলালে তিন repo-তেই একই বদল।
- **Theme contract অলঙ্ঘনীয়, সাইট dark-only।** Tailwind শুধু লেআউটে; চেহারা role class আর `--t-*` টোকেনে।
- **স্ট্যাক:** Next.js 16, React 19, TypeScript, Tailwind v4, react-markdown।

## ডক ইনডেক্স

| ফাইল | দিন | Gist |
|---|---|---|
| [docs/00-rules.md](docs/00-rules.md) | — | লক্ষ্য (২০ আবেদন, ৫ process; সীমা $১,৭০০), সত্যের উৎস, বাজার (ইউরোপ আগে), তিন দরজা (remote-first · ভেটিং · কন্ট্রাক্ট), Ember-এর সুবিধা, সপ্তাহের ছন্দ আর DSA-র সাইট (দিন ০০৮–০৭৭, তিন শনিবারে মহড়া), লেখার বসা, আবেদন ও interview-এর নিয়ম, Dip-এর নিয়ম, যা করবেন না, টাকা আনার ব্যবস্থা, দিন ১৮০-র পরে |
| [docs/01-proof.md](docs/01-proof.md) | ০০১–০৩০ | portfolio, সীমার বাক্য, রিমোট সিভির দুই সংস্করণ, এক মহাদেশের ৩০টা নাম, প্রথম আবেদন দিন ০০৭-এ, টাকা আনার ব্যবস্থা, ৬ STAR, ৯টা ইংরেজি README। শেষে: ৮টা আবেদন |
| [docs/02-writing.md](docs/02-writing.md) | ০৩১–০৬০ | GitHub প্রোফাইল, blog #১ (theme contract), PR description, রিমোট "Tell me about yourself", USD-তে বেতনের তিন উৎস; DSA-র স্ক্রিন-মহড়া #১ দিন ০৩৪-এ। শেষে: ১৭টা আবেদন |
| [docs/03-applications.md](docs/03-applications.md) | ০৬১–০৯০ · dip | দিন ০৭৮-এর মধ্যে ২০টা, দরজা ধরে ফানেল, ওদের টাইমজোনে ২৪ ঘণ্টার উত্তর, ওদের আসল ফিচার নিয়ে design আলোচনা |
| [docs/04-screens.md](docs/04-screens.md) | ০৯১–১২০ · dip | recruiter call-এর ছয় প্রশ্ন (overlap, EOR/contractor, USD), ভেটিং প্ল্যাটফর্মে আবেদন, mock #১। আবেদন সপ্তাহে ২টা |
| [docs/05-technical.md](docs/05-technical.md) | ১২১–১৫০ · dip | live pairing-এর ৬ ধাপ, ৩টা component, Ember বনাম React, frontend system design, blog #২ (hydration), `srdtube`-এর ইংরেজি design doc, take-home মহড়া, mock #২ |
| [docs/06-five-processes.md](docs/06-five-processes.md) | ১৫১–১৮০ · dip | রিমোটের প্রশ্নসহ behavioral, নোট থেকে সিলেবাস, ফানেলের শেষ রায়, রিমোট offer-এর চেকলিস্ট, mock #৩ ও #৪, ইংরেজির তুলনা। শেষে: ২০ আবেদন, ৫ process |

## প্রজেক্ট-নির্দিষ্ট নিয়ম

### তথ্য বদলানোর ক্রম

`brainstorming/ASSUMPTIONS.md` → `brainstorming/` (`crack-remote-company-roadmap.md`, `what-should-i-target-local-or-remote.md`, `two-lakh-per-month-in-2-years.md`, `how-to-write-my-cv.md`, `*-for-remote.md`, `after-getting-response/`) → এই ফোল্ডারের `docs/`।

### ব্লক ফাইলের যে ছাঁচ parser মানে

- `# ব্লক ১ — নাম` — প্রথম H1; "— "-এর পরের অংশ rail-এ দেখায়।
- `*দিন ০০১–০৩০ · dip*` — H1-এর নিচের italic লাইন। শেষে `· dip` থাকলে হোমে Dip-এর সতর্কতা আসে।
- `> **ব্লক শেষে:** …` · `### দিন ০০৭ · শিরোনাম` · `- [ ] ৩০′ …` · `> **দিন শেষে:** …`
- দিনের নম্বর সব ব্লক মিলিয়ে পরপর না হলে build ভাঙে।
- `⚑` = মাইলফলক, `🔁` = ঝালাই হবে, শেষে `🧠 (নাম · নাম)`। নতুন 🧠 নাম লিখলে `app/lib/principles.ts`-এ যোগ করুন — তিন repo-তেই।

### Progress key

| key | মান |
|---|---|
| `src6:v1:start` | শুরুর তারিখ `"YYYY-MM-DD"` |
| `src6:v1:task` | কাজ শেষের তারিখ। id = দিন + কাজের **লেখা** থেকে hash — লেখা বদলালে ঐ কাজের টিক হারায় |
| `src6:v1:check` | দিন শেষ (`d007`) ও ব্লক শেষ (`b1`)-এর হ্যাঁ/না |
| `src6:v1:review` | 🔁 কাজের ঝালাইয়ের অবস্থা `{ base, step }` |

## চালানো

```bash
npm install
npm run dev      # http://localhost:3000
npm run build    # static export → out/
```

push করলে `.github/workflows/deploy.yml` সাইটটা GitHub Pages-এ তোলে।
