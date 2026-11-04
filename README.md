# Dompory Health Academy — expanded release

## Included
11 bilingual pages: home, training, research, about, services, blog, proposals, incubation, nutrition, surveys and epidemiology. Proposed offerings require confirmation of qualifications, capacity, fees, scope and timing. Incubation means initiative mentoring, not clinical/laboratory incubation, investment or guaranteed funding. Outbreak support is training/advisory only, not an emergency service.
Contact: mzamel.health@gmail.com. No payment, backend, upload, student account or automatic mail delivery.

## 1. Preview
Extract the ZIP. Open public/index.html. Keep all public files together.
Design: navy #12304A, teal #007F82, gold #C49A45, off-white #F6F8FA. Gold is decorative, not small body text. English/Arabic switch with RTL; preference stored locally.

## 2. GitHub stores your source
Sign in to github.com. Create a repository (suggested name dompory-health-academy). Upload the extracted CONTENTS, preserving the public folder, firebase.json, README.md and .gitignore. Commit. Use Add file > Upload files for subsequent changes. Never upload private CVs, passwords, patient data or donor-confidential information. A public repository exposes its contents. Saving to GitHub does NOT automatically publish to Firebase.
For this service-oriented academy, use Firebase for production. GitHub Pages is not intended/allowed as free hosting for running an online business or websites primarily facilitating commercial transactions. If you instead create a genuinely noncommercial educational site, review Pages policy; it can publish from main / root or /docs. This package uses /public, not /docs, and is not configured for Pages.

## 3. Free Google hosting: Firebase Hosting (Spark)
Choose Firebase Hosting, NOT Firebase App Hosting (which requires billing). Spark has no-cost quotas, not unlimited hosting. Stay on Spark if avoiding paid usage; service may be limited/stopped at quota. A custom purchased domain is optional; web.app and firebaseapp.com subdomains are provided.
A. Create a Firebase project in the Firebase console. Select Spark; no Analytics needed. Enable Hosting if prompted.
B. Install a currently supported Node.js LTS and the Firebase CLI on your computer.
C. Open a terminal in the extracted folder containing firebase.json (not inside public). Run:

    npm install -g firebase-tools
    firebase login
    firebase use --add

Select the Firebase project and assign alias default. If you prefer the standard setup wizard, run firebase init hosting instead: select the existing project, public directory = public, single-page app = No, automatic GitHub deploy = No, overwrite existing index.html = No. Keep the provided pages and configuration.
D. Deploy:

    firebase deploy --only hosting

Open the actual Hosting URL printed by Firebase. Future updates: edit files, optionally commit/push GitHub, then rerun deploy. GitHub changes do not deploy by themselves in this manual workflow.

## 4. Blogger / domopry
Do not infer an address from the blog display name. Open Blogger, choose your blog and use View blog; copy the visitor URL. The previously supplied blogger.com/blog/posts/... is the owner dashboard, not the visitor URL.
Edit public/config.js and set blogPublicUrl to the confirmed HTTPS visitor address. Redeploy. The article button stays hidden until a valid public URL is configured.
In Blogger: Layout > edit the Pages gadget > Add external link. Title: Academy website. URL: your actual Firebase site URL. Save the link and layout. If the Pages gadget is missing, add it through Layout > Add a Gadget > Pages.
This is two-way navigation, NOT shared login, content synchronisation, migration or automatic importing. This HTML package is NOT a Blogger XML theme. Back up the Blogger theme before unrelated theme edits.

## 5. Final launch checklist
Review both languages, founder titles/qualifications, links, mobile layout and keyboard/dialog behaviour. The supplied CV supports personal experience, not institutional endorsement or academy delivery statistics. No funding, publication, clinical outcome or accreditation guarantees. Validate survey ethics, consent, sampling and data handling before fieldwork. Do not email participant-identifiable data. Confirm nutrition/outbreak advisory boundaries. No legal/privacy compliance certification is provided. Local link checks do not replace browser testing.

## Official documentation
Firebase: https://firebase.google.com/docs/hosting/quickstart
Firebase plans: https://firebase.google.com/support/faq
GitHub limits: https://docs.github.com/pages/getting-started-with-github-pages/github-pages-limits
Blogger pages: https://support.google.com/blogger/answer/165955

## ملخص عربي
فك الضغط وافتح public/index.html للمعاينة. GitHub لحفظ الملفات، Firebase Hosting لنشر الموقع، وBlogger للمقالات. أنشئ مشروع Spark، وثبت Node.js وأداة Firebase، ثم نفذ أوامر الدخول واختيار المشروع والنشر أعلاه من مجلد firebase.json. حافظ على public كمجلد النشر ولا توافق على استبدال index.html. أضف رابط المدونة العام في public/config.js ثم أعد النشر. في Blogger أضف رابط الموقع كرابط خارجي في أداة الصفحات. لا حاجة لشراء نطاق للبدء. لا توجد مزامنة تلقائية مع GitHub في هذا الإعداد.
