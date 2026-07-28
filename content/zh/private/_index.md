---
title: 站点架构
type: landing
summary: 私域 · 仅我可见的站点架构监控页
sections:
  - block: markdown
    content:
      title: ''
      subtitle: ''
      text: |
        <style>
          .priv-wrap{background:#14161c;color:#e7e5df;border-radius:16px;padding:32px;margin:-1rem 0 2rem 0;}
          .priv-wrap h2{color:#f2b56b;font-size:20px;margin:0 0 4px 0;}
          .priv-wrap .priv-sub{color:#9c9a92;font-size:13px;margin:0 0 24px 0;}
          .priv-wrap .priv-badge{display:inline-block;background:#3d2b12;color:#f2b56b;border:1px solid #6b4a1f;border-radius:999px;padding:2px 10px;font-size:12px;margin-bottom:16px;}
          .priv-wrap section{margin-bottom:36px;}
          .priv-wrap h3{color:#7fd1c3;font-size:15px;margin:0 0 12px 0;}
          .priv-wrap svg text{fill:#e7e5df;}
          .priv-wrap svg .muted{fill:#9c9a92;}
        </style>
        <div class="priv-wrap">
          <span class="priv-badge">🔒 管理员视图 · 仅我可见</span>
          <h2>caotianyu.com 站点架构</h2>
          <p class="priv-sub">这个页面本身受 Cloudflare Access 保护（仅我），配色也和公开页面不同 —— 看到这个深色版面，就说明现在是在私域。</p>

          <section>
            <h3>访问权限分层</h3>
            <svg width="100%" viewBox="0 0 640 300" role="img">
              <title>三层访问权限</title>
              <rect x="20" y="20" width="600" height="70" rx="10" fill="#1c3a33" stroke="#2f6e5e" stroke-width="1"/>
              <text x="36" y="45" font-size="14" font-weight="600" fill="#7fd1c3">公开 · 任何人可访问</text>
              <text x="36" y="65" font-size="12" class="muted">学术主页 · 博客 · 旅行 · 爱好 · Kuma 状态页</text>

              <rect x="20" y="105" width="600" height="70" rx="10" fill="#3a2f14" stroke="#6e5a2f" stroke-width="1"/>
              <text x="36" y="130" font-size="14" font-weight="600" fill="#f2b56b">家人朋友 · 需要登录</text>
              <text x="36" y="150" font-size="12" class="muted">生活主页 · Jellyfin(访客账号) · Kavita(访客账号)</text>

              <rect x="20" y="190" width="600" height="70" rx="10" fill="#3a1f1f" stroke="#6e2f2f" stroke-width="1"/>
              <text x="36" y="215" font-size="14" font-weight="600" fill="#e08a8a">仅我 · Cloudflare Access 拦截</text>
              <text x="36" y="235" font-size="12" class="muted">Homepage 管理 · Paperless · Open WebUI · ComfyUI · Whisper · 本页面</text>
            </svg>
          </section>

          <section>
            <h3>页面链接深度（访客点几次能到）</h3>
            <svg width="100%" viewBox="0 0 640 260" role="img">
              <title>站内导航深度</title>
              <rect x="260" y="10" width="120" height="36" rx="6" fill="#22252e" stroke="#454956"/>
              <text x="320" y="33" font-size="12" text-anchor="middle">caotianyu.com</text>

              <line x1="320" y1="46" x2="320" y2="70" stroke="#454956"/>
              <rect x="250" y="70" width="140" height="36" rx="6" fill="#22252e" stroke="#454956"/>
              <text x="320" y="93" font-size="12" text-anchor="middle">/life/ 生活主页</text>
              <text x="410" y="93" font-size="11" class="muted">1 次点击</text>

              <line x1="320" y1="106" x2="130" y2="140" stroke="#454956"/>
              <line x1="320" y1="106" x2="320" y2="140" stroke="#454956"/>
              <line x1="320" y1="106" x2="510" y2="140" stroke="#454956"/>

              <rect x="60" y="140" width="140" height="36" rx="6" fill="#22252e" stroke="#454956"/>
              <text x="130" y="163" font-size="12" text-anchor="middle">/blog/ 列表</text>

              <rect x="250" y="140" width="140" height="36" rx="6" fill="#22252e" stroke="#454956"/>
              <text x="320" y="163" font-size="12" text-anchor="middle">/travel/ 列表</text>

              <rect x="440" y="140" width="140" height="36" rx="6" fill="#22252e" stroke="#454956"/>
              <text x="510" y="163" font-size="12" text-anchor="middle">/sailing 等爱好</text>
              <text x="600" y="163" font-size="11" class="muted">2</text>

              <line x1="130" y1="176" x2="130" y2="200" stroke="#454956"/>
              <line x1="320" y1="176" x2="320" y2="200" stroke="#454956"/>

              <rect x="60" y="200" width="140" height="36" rx="6" fill="#22252e" stroke="#454956"/>
              <text x="130" y="223" font-size="12" text-anchor="middle">具体文章</text>

              <rect x="250" y="200" width="140" height="36" rx="6" fill="#22252e" stroke="#454956"/>
              <text x="320" y="223" font-size="12" text-anchor="middle">/travel/hawaii/</text>
              <text x="410" y="223" font-size="11" class="muted">3 次点击</text>
            </svg>
            <p style="color:#9c9a92;font-size:12px;margin-top:12px;">电影(Jellyfin)、书籍(Kavita) 从 /life/ 直接外链跳出，不计入这棵树，但访问方式已在上面的权限图里标出。</p>
          </section>

          <section>
            <h3>待办</h3>
            <p style="font-size:13px;color:#c7c5bd;">
              · Jellyfin 访客只读账号 + Tailscale Funnel（暂缓）<br>
              · Kavita 访客只读账号<br>
              · 生活主页配色统一（当前用的是学术主页默认配色）
            </p>
          </section>
        </div>
    design:
      columns: '1'
---
