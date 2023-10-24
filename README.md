# CloudflareLink

Cloudflare kullanarak web hook üzerinden eklenen linkleri key store vasıtasıyla redirect eder.

**INDATA 2023**

Uygulamayı publish etmek için
- wrangler publish

Kısa link namespace (key stoere tek bir kez) oluşturma
- wrangler kv:namespace create SHORT_URLS --preview [false]

kısa link bağlama 
- wrangler kv:key put --binding SHORT_URLS "/twitter" "https://twitter.com/nikolalsvk" --preview false