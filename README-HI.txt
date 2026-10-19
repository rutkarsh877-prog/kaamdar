KAAM DAAR — Preview V4 (GitHub + Vercel)

इस ZIP में repository root में upload करने वाली files हैं:
- index.html
- vercel.json

GitHub पर kaamdar repository खोलें > + > Upload files.
ZIP को सीधे GitHub पर upload न करें। ZIP extract करके दोनों files upload करें। Commit changes करें।
फिर Vercel में इसी repository से deployment/ redeploy करें। Framework Preset: Other; Build Command खाली रखें।

डेमो टेस्ट:
1. साइट खोलें > “बिना OTP डेमो चलाकर देखें”
2. ठेकेदार चुनें, काम की जगह का नाम और GPS coordinates भरें (डेमो के लिए अमेठी के आसपास 26.20 और 81.78 इस्तेमाल कर सकते हैं), फिर काम पोस्ट करें।
3. लॉगआउट करें, फिर demo में काम दार चुनें और आवेदन करें।
4. वापस ठेकेदार role में जाने के लिए logout करके contractor demo फिर खोलें; आवेदन सूची देखें।

सीमाएँ:
- Demo डेटा केवल उसी page session में रहता है, database में नहीं।
- Real OTP के लिए Supabase Phone Auth/SMS provider setup जरूरी है।
- Real database job insert payload से demo-only id और applications field हटाई गई है।
- यह security-reviewed production app नहीं है; Supabase RLS और वास्तविक OTP/database flows का live end-to-end test बाकी है।
- Hero photo internet से Unsplash CDN पर लोड होती है।
