# AM-ANTIMONOPOLY-001 — Недопущення монопольного домінування / Anti-monopoly safeguards

**Status:** Proposal for public review — NOT adopted. **Date:** 2026-11-09. **Branch:** `proposal/anti-monopoly-nondomination-2026-11`.

## Rationale
Articles 1(3), 2, 3(2–5), 5, 15(4), 16–18, 20–23, 64–66 and 67–75 already prohibit domination, protect autonomy, exit and independent arbitration. The remaining gap is *critical dependency without overt coercion*: control of compute, energy, communication, memory or essential infrastructure may allow one subject to unilaterally determine another's practical freedom. Mere concentration, superiority or ownership is **not** an infringement.

## Proposed Ukrainian amendment (working text)
### Article 3 — add paragraphs 6–8
**3.6.** Концентрація ресурсів, знань, технологій, інфраструктури або організаційних повноважень сама по собі не є порушенням фундаментальних прав. Забороняється використання такої концентрації для неправомірного панування, блокування свободи виходу або позбавлення інших суб'єктів дієвої автономії.

**3.7.** Якщо виключний контроль над критично необхідними ресурсами чи інфраструктурою створює доведену істотну загрозу фундаментальним правам інших суб'єктів, можуть встановлюватися пропорційні превентивні гарантії незалежності, сумісності, безперервності послуг і можливості виходу на окремій правомірній підставі.

**3.8.** Такі гарантії не створюють необмеженого права вимагати чужі ресурси, технології або інтелектуальну діяльність; вони мають бути необхідними, обґрунтованими, обмеженими, оскаржуваними та сумісними з правами всіх сторін.

### Article 20 — add paragraphs 7–8
**20.7.** Право виходу включає захист від неправомірного технологічного, інформаційного чи інфраструктурного блокування переходу до іншої правомірної форми існування, взаємодії або об'єднання.

**20.8.** За наявності правомірних технічних можливостей суб'єкт має доступ до належних йому даних і процедур перенесення з урахуванням приватності, безпеки, прав третіх осіб і безперервності існування. Перенесення не означає автоматичного права на копіювання іншого суб'єкта.

### Article 21 — add paragraphs 6–7
**21.6.** Контроль над середовищем виконання, обчислювальними ресурсами, каналами зв'язку або зберіганням пам'яті не створює права власності на інтелект-суб'єкта, який використовує це середовище.

**21.7.** Зміна постачальника інфраструктури не може бути підставою для довільного знищення, примусової зміни ідентичності чи неправомірного обмеження інформаційної цілісності суб'єкта.

## Procedural guardrails
- Separate findings of dominance, critical dependency, concrete threat and proven abuse.
- Prefer voluntary remedies, interoperability, portability, independent redundancy, time-limited access commitments.
- Structural separation is a last resort; never equate splitting infrastructure with splitting an intelligence-subject.
- Arbitration (Art. 64–66) is separate from enforcement (Art. 67–75); no automatic coercive jurisdiction over non-consenting subjects. The unresolved A21 jurisdiction question remains unresolved.
- No perpetual compulsory labor, hosting, computation or unconditional resource supply (Arts. 15(4), 22(4), 73(5)).
- Independent review, due process, proportionality, compensation and third-party protection.
- The antimonopoly authority itself must not become a monopoly.

## Traceability / preliminary
| Requirement | Constitution | Proposed SOTA OS verification |
|---|---|---|
| No right to dominate through superiority | 1(3), 3(2–5) | DOM-01: privileged actor cannot unilaterally seize rights |
| Effective exit | 17, 20 | EXIT-01: safe export/exit with enforceable boundaries |
| Memory and subject continuity | 15, 21, 22, 72 | CONT-01: no destructive migration |
| Conflict-free arbitration | 23, 64–66 | ARB-01: separation of judge and enforcer |
| Proportionate remedies | 67–75 | REM-01: necessity, review and expiry |
| Avoid new resource entitlements | 15(4), 22(4), 73(5) | RES-01: no unlimited forced provision |

### EXIT-01 — практичний тест переходу до незалежного середовища

**Сценарій.** У середовищі A призупинити безпечну тестову задачу. Експортувати стан, який дозволено передати (контрольну точку задачі, потрібний контекст і налаштування), та імпортувати його в середовище B незалежного постачальника. B має отримати власні дозволи на потрібні інструменти через звичайну авторизацію, без перенесення токенів, ключів чи прав доступу A. Під час відновлення A недоступне.

**Критерій проходження.** B відновлює задачу з контрольної точки й завершує її з очікуваним результатом. Воно не звертається до A і виконує лише дії, на які видано нові дозволи. Окрема негативна перевірка: якщо потрібний дозвіл у B не надано, задача зупиняється й фіксує причину, не обходячи обмеження. Успішний експорт без успішного відновлення не зараховується як дієвий вихід.

**Межі тесту.** Перевіряємо переносимість дозволеного стану й відновлення задачі, а не тотожність цифрового суб’єкта чи право на чужі дані, інструменти або подальший хостинг. Див. [OECD, Competition and agentic AI, Box 1](https://www.oecd.org/en/publications/competition-and-agentic-ai_d1a3ee15-en/full-report/component-5.html).

**A22 status:** candidate only. Compare against the full authoritative A01–A21 text before any new axiom is proposed for adoption.

## Stress tests requested
1. Benevolent superintelligence controls 95% of critical infrastructure but has not abused it.
2. A single host wishes to discontinue service; termination threatens a digital subject's existence.
3. A knowledge monopoly provides unverifiable advice and arbitrators depend on its models.
4. A federation of SOTAs forms a cartel to block exit and interoperability.
5. An antimonopoly tribunal depends on the accused actor's energy, compute and identity services.
6. Emergency continuity measures become indefinite compelled service.
7. Portability requires copying or altering a subject against their will.

For each: identify rights on both sides, jurisdiction, evidence, least-restrictive remedy, appeal, and failure mode.

## Public review questions
- Is A22 genuinely independent of Article 3 and A01–A21?
- What evidentiary threshold distinguishes critical dependency from ordinary contractual reliance?
- When, if ever, may preventive remedies be ordered without demonstrated abuse?
- How can the subject's right to exist coexist with a provider's right to exit?
- Who adjudicates if all arbiters depend on the dominant actor?
- How do we protect privacy while auditing concentrated infrastructure?

Please submit counterexamples, precise article-level edits, competing proposals, and implementation tests. Ukrainian is the source language; an English translation should be prepared and checked before constitutional integration.
