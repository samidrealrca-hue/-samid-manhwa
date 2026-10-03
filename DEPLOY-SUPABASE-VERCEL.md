
# نشر SAMID MANHWA — Vercel + Supabase

## 1) Supabase
1. أنشئ مشروعًا جديدًا في Supabase.
2. افتح SQL Editor.
3. الصق محتوى `supabase/schema.sql` وشغّله.
4. من Project Settings > API انسخ:
   - Project URL
   - anon/public key

## 2) Vercel
1. ارفع المشروع إلى GitHub.
2. في Vercel اختر Add New Project ثم اختر مستودع SAMID MANHWA.
3. أضف Environment Variables:
   `NEXT_PUBLIC_SUPABASE_URL`
   `NEXT_PUBLIC_SUPABASE_ANON_KEY`
4. Deploy.

## 3) Admin
هذه النسخة هي Starter جاهز للربط. لا تستخدم service_role key في المتصفح.
المرحلة التالية بعد الربط هي بناء Admin Auth كامل ورفع الصور إلى Supabase Storage مع سياسات RLS.

## 4) الرابط وQR
بعد نجاح Deploy سيعطيك Vercel رابطًا مثل:
`https://samid-manhwa-xxxx.vercel.app`
يمكن بعد ذلك إنشاء QR Code لهذا الرابط.
