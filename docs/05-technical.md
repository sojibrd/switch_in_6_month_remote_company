# ব্লক ৫ — take-home, pairing আর লেখা design

*দিন ১২১–১৫০ · dip*

রিমোটে কারিগরি রাউন্ড সাধারণত দুই রূপে আসে। **লিখিত** — take-home, সাথে "কেন এই সিদ্ধান্ত" বা একটা ছোট design doc; পাঁচ টাইমজোনের টিম সিদ্ধান্ত লিখেই রাখে। **আলোচনামূলক** — shared editor-এ live pairing, বা *"আমাদের এই ফিচারটা আপনি কীভাবে বানাতেন?"* নতুন DSA নয়: pairing-এর অনুশীলন ৫০টার ঝালাই দিয়েই, জোরে, ইংরেজিতে।

রিমোট frontend পদে সবচেয়ে সম্ভাব্য design প্রশ্ন **frontend system design** — component, state, ডেটা আনা ও cache, optimistic update, accessibility। আর `srdtube`-এর **ইংরেজি design doc** — লোকালে যা প্রস্তুতি, রিমোটে তা জমা দেওয়ার মতো নমুনা। দুটোই হয় [রিমোট system design](https://sojibrd.github.io/system_design_remote_company/)-এ (এই plan-এর দিন ১০৬–১৩৩); এই ব্লকে ওগুলো মুখে।

মাইলফলক: ইংরেজি design doc প্রকাশ দিন ১২৪-এ (system design সাইটে), mock #২ দিন ১৩৯-এ, blog #২ প্রকাশ দিন ১৪৩-এ।

> **ব্লক শেষে:** pairing-এর ৬ ধাপ মুখস্থ, mock #২ হয়েছে, ৩টা component, blog #২ আর ইংরেজি design doc প্রকাশিত?

### দিন ১২১ · আবেদন

- [ ] ৩০′ আগে আজকের ঝালাই — এখন থেকে জোরে, ইংরেজিতে, pairing-এর ধাপে, ১৫′-এর মধ্যে; তারপর [রিমোট system design](https://sojibrd.github.io/system_design_remote_company/)-এর আজকের দিন 🧠 (Spaced repetition · Deliberate practice)
- [ ] ৩০′ আবেদন — সপ্তাহের ১ম 🧠 (System vs goal)
- [ ] ১৫′ ইংরেজি — কোন কোন রাউন্ড হবে, প্রথম কলে কীভাবে জিজ্ঞেস করবেন

> **দিন শেষে:** আবেদন গেছে?

### দিন ১২২ · pairing-এর ৬ ধাপ

- [ ] ৩০′ আগে আজকের ঝালাই, ১৫′-এর মধ্যে; তারপর [রিমোট system design](https://sojibrd.github.io/system_design_remote_company/)-এর আজকের দিন 🧠 (Spaced repetition · Deliberate practice)
- [ ] ২৫′ live pairing-এর **৬ ধাপ** একটা কার্ডে, ইংরেজি বাক্যসহ: ১) নিজের ভাষায় আবার বলা *"So I need to… is that right?"* ২) input নিয়ে ২টা প্রশ্ন ৩) ছোট উদাহরণ হাতে ৪) সহজ সমাধান আগে, তারপর ভালোটা ৫) কোড, মুখে বলতে বলতে ৬) উদাহরণে পরীক্ষা + complexity 🔁 🧠 (Chunk the subject)
- [ ] ১৫′ ইংরেজি — কার্ড না দেখে ৬ ধাপ বলুন

> **দিন শেষে:** ৬ ধাপ না দেখে বলা যায়?

### দিন ১২৩ · আবেদন

- [ ] ৩০′ আগে আজকের ঝালাই — ৬ ধাপে, জোরে, ১৫′-এর মধ্যে; তারপর [রিমোট system design](https://sojibrd.github.io/system_design_remote_company/)-এর আজকের দিন 🧠 (Spaced repetition · Deliberate practice)
- [ ] ৩০′ আবেদন — সপ্তাহের ২য়
- [ ] ১৫′ ইংরেজি — আটকে গেলে: *"I'm stuck between two approaches — could I get a hint?"* — পাঁচবার

> **দিন শেষে:** সপ্তাহের দুটো আবেদন গেছে?

### দিন ১২৪ · follow-up

- [ ] ৩০′ আগে আজকের ঝালাই — ৬ ধাপে, জোরে, ১৫′-এর মধ্যে; তারপর [রিমোট system design](https://sojibrd.github.io/system_design_remote_company/)-এর আজকের দিন 🧠 (Spaced repetition · Deliberate practice)
- [ ] ১৫′ LinkedIn বার্তা ×১ · ৭–১০ দিন আগের আবেদনে একবার follow-up
- [ ] ১৫′ ইংরেজি — আজকের ঝালাইয়ে কোন ধাপে চুপ হয়ে গেলেন

> **দিন শেষে:** follow-up গেছে?

### দিন ১২৫ · component ১ — debounced search

- [ ] ৪৫′ **Debounced search** — React + TS, ফাঁকা ফাইল থেকে, টাইমার ৪৫′: input, ৩০০ms debounce, পুরনো request বাতিল (AbortController), loading ও empty অবস্থা 🔁 🧠 (Deliberate practice · Parkinson's law)
- [ ] ১৫′ ইংরেজি — কেন debounce, কেন পুরনো request বাতিল — কোড দেখিয়ে জোরে, যেন pairing-এ

> **দিন শেষে:** ৪৫ মিনিটে কাজ করল?

### দিন ১২৬ · framework ১ — reactivity

- [ ] ১০′ সপ্তাহের হিসাব
- [ ] ৩৫′ **Ember-এর autotracking বনাম React-এর re-render** — বাচ্চাকে বোঝানোর মতো ৮–১০ লাইনে, ইংরেজিতে; যেখানে আটকালেন, সেখানে ফিরে গিয়ে আবার। Ember পদে এটাই আপনার বিরল জায়গা 🔁 🧠 (Feynman · Trunk based knowledge)
- [ ] ১৫′ ইংরেজি — লেখাটা না দেখে ২ মিনিটে, রেকর্ড

> **দিন শেষে:** না দেখে ২ মিনিট বলা গেছে?

### দিন ১২৭ · বার্তা

- [ ] ৩০′ আগে আজকের ঝালাই — ৬ ধাপে, জোরে, ১৫′-এর মধ্যে; তারপর [রিমোট system design](https://sojibrd.github.io/system_design_remote_company/)-এর আজকের দিন 🧠 (Spaced repetition · Deliberate practice)
- [ ] ১৫′ LinkedIn বার্তা ×২
- [ ] ১৫′ ইংরেজি — *"In Ember we'd solve this with…; in React I'd use…"* — একটা উদাহরণ বানিয়ে বলুন

> **দিন শেষে:** বার্তা দুটো গেছে?

### দিন ১২৮ · আবেদন

- [ ] ৩০′ আগে আজকের ঝালাই — ৬ ধাপে, জোরে, ১৫′-এর মধ্যে; তারপর [রিমোট system design](https://sojibrd.github.io/system_design_remote_company/)-এর আজকের দিন 🧠 (Spaced repetition · Deliberate practice)
- [ ] ৩০′ আবেদন — সপ্তাহের ১ম
- [ ] ১৫′ ইংরেজি — debounced search-এর ব্যাখ্যা, কোড ছাড়া

> **দিন শেষে:** আবেদন গেছে?

### দিন ১২৯ · framework ২ — state কোথায়

- [ ] ৩০′ আগে আজকের ঝালাই, ১৫′-এর মধ্যে; তারপর [রিমোট system design](https://sojibrd.github.io/system_design_remote_company/)-এর আজকের দিন 🧠 (Spaced repetition · Deliberate practice)
- [ ] ২৫′ **কোন state কোথায়** — component, service, নাকি URL; তিনটার প্রতিটায় নিজের কাজ থেকে একটা উদাহরণ, আর ভুল জায়গায় রাখলে কী ভাঙে 🔁 🧠 (Feynman · Concepts vs Facts)
- [ ] ১৫′ ইংরেজি — উদাহরণ তিনটা জোরে

> **দিন শেষে:** তিনটা জায়গার তিনটা উদাহরণ লেখা?

### দিন ১৩০ · আবেদন

- [ ] ৩০′ আগে আজকের ঝালাই — ৬ ধাপে, জোরে, ১৫′-এর মধ্যে; তারপর [রিমোট system design](https://sojibrd.github.io/system_design_remote_company/)-এর আজকের দিন 🧠 (Spaced repetition · Deliberate practice)
- [ ] ৩০′ আবেদন — সপ্তাহের ২য়
- [ ] ১৫′ ইংরেজি — state-এর প্রশ্ন, ঠান্ডা শুরুতে

> **দিন শেষে:** সপ্তাহের দুটো আবেদন গেছে?

### দিন ১৩১ · follow-up

- [ ] ৩০′ আগে আজকের ঝালাই — ৬ ধাপে, জোরে, ১৫′-এর মধ্যে; তারপর [রিমোট system design](https://sojibrd.github.io/system_design_remote_company/)-এর আজকের দিন 🧠 (Spaced repetition · Deliberate practice)
- [ ] ১৫′ LinkedIn বার্তা ×১ · follow-up
- [ ] ১৫′ ইংরেজি — mock #২-এর জন্য সঙ্গীকে সময় নিশ্চিত করার বার্তা, মুখে আগে; এবার shared editor-এ live pairing 🧠 (Community)

> **দিন শেষে:** mock #২-এর সময় দিন ১৩৯-এ নিশ্চিত?

### দিন ১৩২ · component ২ — modal

- [ ] ৪০′ **Modal, focus trap সহ** — খুললে focus ভেতরে, Tab ঘোরে ভেতরেই, Esc-এ বন্ধ, বন্ধ হলে focus আগের বোতামে; টাইমার ৪০′ 🔁 🧠 (Deliberate practice)
- [ ] ২০′ frontend system design — [রিমোট system design](https://sojibrd.github.io/system_design_remote_company/)-এর তিনটা UI-র একটা এলোমেলো তুলে, ছয় ধাপে, ইংরেজিতে জোরে 🧠 (Interleaving · Test yourself)

> **দিন শেষে:** modal-এ keyboard দিয়ে সব কাজ করে?

### দিন ১৩৩ · blog #২ — খসড়া

- [ ] ১০′ সপ্তাহের হিসাব
- [ ] ৩৫′ ইংরেজি **blog post #২ — static export-এ hydration mismatch:** কী ভাঙল, কেন ভাঙল, কী ঠিক করলেন (`localStorage` এক জায়গায় আটকে রাখা), কী শিখলেন; এক পাতা 🧠 (Active learning · Skill stacking)
- [ ] ১৫′ ইংরেজি — খসড়াটা জোরে পড়ুন; যেখানে হোঁচট, সেখানে বাক্য ছোট 🧠 (Feedback)

> **দিন শেষে:** এক পাতার খসড়া আছে?

### দিন ১৩৪ · বার্তা

- [ ] ৩০′ আজকের ঝালাই — ৬ ধাপে, জোরে 🧠 (Spaced repetition)
- [ ] ১৫′ LinkedIn বার্তা ×২
- [ ] ১৫′ ইংরেজি — autocomplete-এর ক্রম, না দেখে

> **দিন শেষে:** বার্তা দুটো গেছে?

### দিন ১৩৫ · আবেদন

- [ ] ৩০′ আজকের ঝালাই — ৬ ধাপে, জোরে 🧠 (Spaced repetition)
- [ ] ৩০′ আবেদন — সপ্তাহের ১ম
- [ ] ১৫′ ইংরেজি — modal-এর accessibility, কেন focus ফেরাতে হয়

> **দিন শেষে:** আবেদন গেছে?

### দিন ১৩৬ · framework ৩ — async

- [ ] ৩০′ আজকের ঝালাই 🧠 (Spaced repetition)
- [ ] ২৫′ **ember-concurrency-র task বনাম React-এর useEffect** — restartable task আর AbortController; দুবার fetch, বাসি data, unmount-এর পরে setState — প্রতিটা কীভাবে ঠেকান 🔁 🧠 (Feynman · Trunk based knowledge)
- [ ] ১৫′ ইংরেজি — ২ মিনিটে, রেকর্ড

> **দিন শেষে:** তিনটা সমস্যার তিনটা উত্তর লেখা?

### দিন ১৩৭ · আবেদন

- [ ] ৩০′ আজকের ঝালাই — ৬ ধাপে, জোরে 🧠 (Spaced repetition)
- [ ] ৩০′ আবেদন — সপ্তাহের ২য়
- [ ] ১৫′ ইংরেজি — async-এর তিন সমস্যা, ৯০ সেকেন্ডে

> **দিন শেষে:** সপ্তাহের দুটো আবেদন গেছে?

### দিন ১৩৮ · হালকা দিন

- [ ] ১৫′ follow-up — ৭–১০ দিন আগের আবেদনে
- [ ] ১৫′ ইংরেজি — কাল mock; আজ শুধু ৬ ধাপ একবার, তারপর বন্ধ 🧠 (Sleep · It pays to be not busy)

> **দিন শেষে:** কালকের mock-এর সময় নিশ্চিত?

### দিন ১৩৯ · mock interview #২

- [ ] ৪৫′ ⚑ **mock interview #২ — live pairing** — shared editor-এ, সঙ্গী ৫০টার মধ্যে থেকে একটা বাছবে (**আপনি নয়**), ৩০ মিনিট, ৬ ধাপে, ইংরেজিতে জোরে ভেবে; তারপর একটা frontend প্রশ্ন; রেকর্ড 🧠 (Test yourself · Interleaving)
- [ ] ১৫′ ৫ লাইনের নোট — কোন ধাপে চুপ হলেন, hint চাইলেন কিনা, সঙ্গী কী বলল, পরের বার একটা জিনিস 🧠 (Feedback · Failures don't count)

> **দিন শেষে:** mock #২ হয়েছে, নোট লেখা?

### দিন ১৪০ · design doc মুখে — ১

- [ ] ১০′ সপ্তাহের হিসাব
- [ ] ৩৫′ `srdtube`-এর ইংরেজি design doc **মুখে**, doc বন্ধ — প্রথম তিন সেকশন: **কী বানিয়েছি · কতজন ব্যবহারকারী ধরে · কোন সিদ্ধান্ত কেন**; রেকর্ড। লেখা ও প্রকাশ হয়েছে [রিমোট system design](https://sojibrd.github.io/system_design_remote_company/)-এ 🧠 (Test yourself · Active learning)
- [ ] ১৫′ ইংরেজি — mock #২-এর "একটা জিনিস" নিয়ে একটা প্রবলেম আবার, জোরে 🧠 (Deliberate practice)

> **দিন শেষে:** তিন সেকশন doc ছাড়া বলা গেছে?

### দিন ১৪১ · বার্তা

- [ ] ৩০′ আজকের ঝালাই — ৬ ধাপে, জোরে 🧠 (Spaced repetition)
- [ ] ১৫′ LinkedIn বার্তা ×২
- [ ] ১৫′ ইংরেজি — `srdtube`-এর তিনটা সিদ্ধান্ত, ১ মিনিটে

> **দিন শেষে:** বার্তা দুটো গেছে?

### দিন ১৪২ · আবেদন

- [ ] ৩০′ আজকের ঝালাই — ৬ ধাপে, জোরে 🧠 (Spaced repetition)
- [ ] ৩০′ আবেদন — সপ্তাহের ১ম
- [ ] ১৫′ ইংরেজি — reactivity-র প্রশ্ন, ঠান্ডা শুরুতে

> **দিন শেষে:** আবেদন গেছে?

### দিন ১৪৩ · blog #২ প্রকাশ

- [ ] ৩০′ আজকের ঝালাই 🧠 (Spaced repetition)
- [ ] ২৫′ ⚑ **blog #২ প্রকাশ** — শেষবার ঠিক করে প্রকাশ; portfolio আর GitHub প্রোফাইল থেকে লিংক। নিখুঁত নয়, প্রকাশিত 🧠 (Have an endpoint · Failures don't count)
- [ ] ১৫′ ইংরেজি — hydration-এর গল্প, ৯০ সেকেন্ডে

> **দিন শেষে:** blog #২-এর লিংক portfolio-তে আছে?

### দিন ১৪৪ · আবেদন

- [ ] ৩০′ আজকের ঝালাই — ৬ ধাপে, জোরে 🧠 (Spaced repetition)
- [ ] ৩০′ আবেদন — সপ্তাহের ২য়; চিঠির প্রমাণ = blog #২
- [ ] ১৫′ ইংরেজি — "Tell me about a bug you're proud of fixing"

> **দিন শেষে:** সপ্তাহের দুটো আবেদন গেছে?

### দিন ১৪৫ · follow-up

- [ ] ৩০′ আজকের ঝালাই — ৬ ধাপে, জোরে 🧠 (Spaced repetition)
- [ ] ১৫′ LinkedIn বার্তা ×১ · follow-up
- [ ] ১৫′ ইংরেজি — ember-concurrency বনাম useEffect, ঠান্ডা শুরুতে

> **দিন শেষে:** follow-up গেছে?

### দিন ১৪৬ · take-home মহড়া

- [ ] ৫০′ take-home মহড়া — **পাতা ভাগ করা table, খোঁজা সহ**; নিজেকে ৫০′-এর কড়া সীমা, দিন ১১৫-এর চেকলিস্ট মেনে জমা: README-তে সিদ্ধান্ত, "সময় থাকলে আর কী", আর ইংরেজিতে ৫ লাইনের design note 🔁 🧠 (Parkinson's law · Deliberate practice)
- [ ] ১০′ ইংরেজি — design note-টা জোরে

> **দিন শেষে:** সীমার মধ্যে জমা হলো, বাড়তি ফিচার ছাড়া?

### দিন ১৪৭ · design doc মুখে — ২

- [ ] ১০′ সপ্তাহের হিসাব
- [ ] ৩৫′ `srdtube`-এর doc মুখে, বাকি তিনটা — **কী বাদ দিয়েছি · গঠনটা কেমন · কোথায় ভাঙবে**; শেষে তিন রিমোট প্রশ্ন, doc বন্ধ: *"Why this and not the alternative?" · "What did you deliberately leave out?" · "Availability or consistency here — which, and why?"*; রেকর্ড 🧠 (Test yourself · Einstellung)
- [ ] ১৫′ ইংরেজি — "কোথায় ভাঙবে" সেকশন, সহজ উত্তর আগে, তারপর *"Would you like more detail?"*

> **দিন শেষে:** ছয় সেকশন আর তিন প্রশ্ন doc ছাড়া বলা গেছে?

### দিন ১৪৮ · বার্তা

- [ ] ৩০′ আজকের ঝালাই — ৬ ধাপে, জোরে 🧠 (Spaced repetition)
- [ ] ১৫′ LinkedIn বার্তা ×২ — design doc-এর লিংক সাথে
- [ ] ১৫′ ইংরেজি — design doc-এর "কী বাদ দিয়েছি", ১ মিনিট

> **দিন শেষে:** বার্তা দুটো গেছে?

### দিন ১৪৯ · আবেদন

- [ ] ৩০′ আজকের ঝালাই — ৬ ধাপে, জোরে 🧠 (Spaced repetition)
- [ ] ৩০′ আবেদন — সপ্তাহের ১ম; চিঠির প্রমাণ = design doc
- [ ] ১৫′ ইংরেজি — take-home-এর একটা সিদ্ধান্ত, কেন

> **দিন শেষে:** আবেদন গেছে?

### দিন ১৫০ · component ৩ — tabs, আর হিসাব

- [ ] ২৫′ **Tabs, keyboard navigation সহ** — ← → দিয়ে tab বদল, Home/End, `role="tablist"` আর `aria-selected`; টাইমার ২৫′ 🔁 🧠 (Deliberate practice)
- [ ] ১৫′ ব্লক ৫-এর হিসাব — ৬ ধাপ, mock #২, ৩টা component, take-home মহড়া, blog #২, design doc, framework-এর ৩ প্রশ্ন: কোনটা বাকি, "এখনো ___-এ আছি" 🧠 (It's all in the frame)
- [ ] ১৫′ ইংরেজি — এই ব্লকে সবচেয়ে কঠিন যেটা ছিল, সেটা এখন কেমন লাগে

> **দিন শেষে:** ব্লক ৫ — pairing-এর ৬ ধাপ মুখস্থ আর mock #২ হয়েছে?
