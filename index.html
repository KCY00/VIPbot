<!DOCTYPE html>
<html lang="zh-CN">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>TG Bot 控制台</title>
<link href="https://fonts.googleapis.com/css2?family=Space+Mono:wght@400;700&family=Syne:wght@400;600;700;800&display=swap" rel="stylesheet">
<style>
  :root {
    --bg:#0a0a0f;--surface:#111118;--surface2:#1a1a24;--border:#2a2a3a;
    --accent:#00e5a0;--accent2:#7c6af7;--accent3:#ff6b6b;--accent4:#ffd166;
    --text:#e8e8f0;--text-dim:#6e6e8a;--text-muted:#3a3a55;
  }
  *{margin:0;padding:0;box-sizing:border-box;}
  body{font-family:'Syne',sans-serif;background:var(--bg);color:var(--text);min-height:100vh;display:flex;overflow:hidden;}

  /* LOGIN */
  #login-screen{position:fixed;inset:0;background:var(--bg);display:flex;align-items:center;justify-content:center;z-index:999;}
  .login-box{width:420px;background:var(--surface);border:1px solid var(--border);border-radius:20px;padding:40px;position:relative;overflow:hidden;}
  .login-box::before{content:'';position:absolute;top:0;left:0;right:0;height:3px;background:linear-gradient(90deg,var(--accent),var(--accent2));}
  .login-logo{display:flex;align-items:center;gap:14px;margin-bottom:32px;}
  .login-logo-icon{width:48px;height:48px;background:linear-gradient(135deg,var(--accent),var(--accent2));border-radius:14px;display:flex;align-items:center;justify-content:center;font-size:24px;}
  .login-title{font-size:15px;font-weight:700;margin-bottom:6px;}
  .login-desc{font-size:12px;color:var(--text-dim);margin-bottom:24px;line-height:1.6;}
  .login-input-wrap{position:relative;margin-bottom:12px;}
  .login-input{width:100%;padding:12px 44px 12px 14px;background:var(--surface2);border:1px solid var(--border);border-radius:10px;color:var(--text);font-size:13px;font-family:'Space Mono',monospace;outline:none;transition:border-color 0.2s;}
  .login-input:focus{border-color:var(--accent);}
  .login-eye{position:absolute;right:12px;top:50%;transform:translateY(-50%);cursor:pointer;color:var(--text-dim);font-size:16px;user-select:none;}
  .login-hint{font-size:10px;color:var(--text-muted);margin-bottom:20px;font-family:'Space Mono',monospace;}
  .login-hint b{color:var(--accent4);}
  .login-btn{width:100%;padding:12px;border-radius:10px;border:none;background:var(--accent);color:#0a0a0f;font-size:14px;font-weight:800;font-family:'Syne',sans-serif;cursor:pointer;transition:all 0.2s;}
  .login-btn:hover{background:#00ffb3;transform:translateY(-1px);}
  .login-btn:disabled{opacity:0.5;cursor:not-allowed;transform:none;}
  .login-error{background:rgba(255,107,107,0.1);border:1px solid rgba(255,107,107,0.3);border-radius:8px;padding:10px 14px;font-size:12px;color:var(--accent3);margin-bottom:16px;display:none;}
  .login-security{display:flex;align-items:flex-start;gap:10px;margin-top:20px;padding:12px 14px;background:rgba(0,229,160,0.05);border-radius:8px;border:1px solid rgba(0,229,160,0.1);}
  .login-security-text{font-size:10px;color:var(--text-dim);line-height:1.6;}
  .login-security-text b{color:var(--accent);}

  /* SIDEBAR */
  .sidebar{width:240px;background:var(--surface);border-right:1px solid var(--border);display:flex;flex-direction:column;padding:24px 0;flex-shrink:0;position:relative;}
  .sidebar::before{content:'';position:absolute;top:0;left:0;right:0;height:2px;background:linear-gradient(90deg,var(--accent),var(--accent2));}
  .logo{padding:0 24px 32px;display:flex;align-items:center;gap:12px;}
  .logo-icon{width:36px;height:36px;background:linear-gradient(135deg,var(--accent),var(--accent2));border-radius:10px;display:flex;align-items:center;justify-content:center;font-size:18px;}
  .logo-text{font-size:15px;font-weight:800;}
  .logo-sub{font-size:10px;color:var(--text-dim);font-family:'Space Mono',monospace;}
  .nav-label{font-size:9px;font-weight:700;letter-spacing:2px;color:var(--text-muted);text-transform:uppercase;padding:8px 24px 4px;font-family:'Space Mono',monospace;}
  .nav-section{padding:0 12px 8px;margin-top:4px;}
  .nav-item{display:flex;align-items:center;gap:10px;padding:10px 12px;border-radius:8px;cursor:pointer;font-size:13px;font-weight:600;color:var(--text-dim);transition:all 0.15s;position:relative;border:1px solid transparent;}
  .nav-item:hover{color:var(--text);background:var(--surface2);}
  .nav-item.active{color:var(--accent);background:rgba(0,229,160,0.08);border-color:rgba(0,229,160,0.2);}
  .nav-item.active::before{content:'';position:absolute;left:-1px;top:6px;bottom:6px;width:3px;background:var(--accent);border-radius:0 3px 3px 0;}
  .nav-icon{font-size:16px;width:20px;text-align:center;}
  .badge{margin-left:auto;font-size:10px;font-weight:700;background:var(--accent2);color:#fff;padding:2px 6px;border-radius:20px;font-family:'Space Mono',monospace;}
  .bot-status{margin:16px 12px 0;background:var(--surface2);border:1px solid var(--border);border-radius:10px;padding:12px;}
  .bot-status-header{display:flex;align-items:center;gap:8px;margin-bottom:6px;}
  .status-dot{width:8px;height:8px;border-radius:50%;background:var(--accent);box-shadow:0 0 8px var(--accent);animation:pulse 2s infinite;}
  @keyframes pulse{0%,100%{opacity:1}50%{opacity:0.4}}
  .status-label{font-size:11px;font-weight:700;color:var(--accent);}
  .bot-name{font-size:12px;color:var(--text-dim);font-family:'Space Mono',monospace;}
  .bot-token-display{font-size:9px;color:var(--text-muted);font-family:'Space Mono',monospace;margin-top:2px;}
  .logout-btn{margin:10px 12px 0;padding:8px;border-radius:8px;border:1px solid var(--border);background:transparent;color:var(--text-dim);font-size:11px;font-weight:600;font-family:'Syne',sans-serif;cursor:pointer;width:calc(100% - 24px);transition:all 0.15s;}
  .logout-btn:hover{border-color:var(--accent3);color:var(--accent3);}

  /* MAIN */
  .main{flex:1;display:flex;flex-direction:column;overflow:hidden;}
  .topbar{height:60px;background:var(--surface);border-bottom:1px solid var(--border);display:flex;align-items:center;padding:0 28px;gap:16px;flex-shrink:0;}
  .page-title{font-size:18px;font-weight:800;flex:1;}
  .topbar-actions{display:flex;gap:10px;align-items:center;}
  .btn{padding:8px 16px;border-radius:8px;font-size:12px;font-weight:700;font-family:'Syne',sans-serif;cursor:pointer;border:none;transition:all 0.15s;display:flex;align-items:center;gap:6px;}
  .btn-primary{background:var(--accent);color:#0a0a0f;}
  .btn-primary:hover{background:#00ffb3;transform:translateY(-1px);}
  .btn-ghost{background:transparent;color:var(--text-dim);border:1px solid var(--border);}
  .btn-ghost:hover{color:var(--text);border-color:var(--text-dim);}
  .btn-danger{background:rgba(255,107,107,0.15);color:var(--accent3);border:1px solid rgba(255,107,107,0.3);}
  .btn-danger:hover{background:rgba(255,107,107,0.25);}
  .content{flex:1;overflow-y:auto;padding:28px;}
  .content::-webkit-scrollbar{width:6px;}
  .content::-webkit-scrollbar-thumb{background:var(--border);border-radius:3px;}

  /* PAGES */
  .page{display:none;}
  .page.active{display:block;animation:fadeIn 0.2s ease;}
  @keyframes fadeIn{from{opacity:0;transform:translateY(6px)}to{opacity:1;transform:none}}

  /* STATS */
  .stats-grid{display:grid;grid-template-columns:repeat(4,1fr);gap:16px;margin-bottom:24px;}
  .stat-card{background:var(--surface);border:1px solid var(--border);border-radius:12px;padding:20px;position:relative;overflow:hidden;}
  .stat-card::after{content:'';position:absolute;bottom:0;left:0;right:0;height:2px;}
  .stat-card.green::after{background:var(--accent);}
  .stat-card.purple::after{background:var(--accent2);}
  .stat-card.red::after{background:var(--accent3);}
  .stat-card.yellow::after{background:var(--accent4);}
  .stat-icon{font-size:22px;margin-bottom:10px;}
  .stat-value{font-size:22px;font-weight:800;line-height:1;margin-bottom:4px;word-break:break-all;}
  .stat-value.green{color:var(--accent);}
  .stat-value.purple{color:var(--accent2);}
  .stat-value.red{color:var(--accent3);}
  .stat-value.yellow{color:var(--accent4);}
  .stat-label{font-size:10px;color:var(--text-dim);font-weight:600;text-transform:uppercase;letter-spacing:1px;}
  .stat-change{font-size:10px;color:var(--text-muted);margin-top:4px;font-family:'Space Mono',monospace;}

  /* CARDS */
  .charts-row{display:grid;grid-template-columns:2fr 1fr;gap:16px;margin-bottom:24px;}
  .card{background:var(--surface);border:1px solid var(--border);border-radius:12px;overflow:hidden;}
  .card-header{padding:16px 20px;border-bottom:1px solid var(--border);display:flex;align-items:center;justify-content:space-between;}
  .card-title{font-size:13px;font-weight:700;}
  .card-subtitle{font-size:11px;color:var(--text-dim);margin-top:1px;}
  .card-body{padding:20px;}

  /* TABLE */
  .table-wrap{overflow-x:auto;}
  table{width:100%;border-collapse:collapse;}
  thead tr{border-bottom:1px solid var(--border);}
  thead th{padding:10px 16px;text-align:left;font-size:10px;font-weight:700;letter-spacing:1.5px;text-transform:uppercase;color:var(--text-dim);font-family:'Space Mono',monospace;}
  tbody tr{border-bottom:1px solid rgba(42,42,58,0.5);transition:background 0.15s;}
  tbody tr:hover{background:rgba(255,255,255,0.02);}
  tbody td{padding:12px 16px;font-size:13px;color:var(--text);}
  .user-cell{display:flex;align-items:center;}
  .user-avatar{width:28px;height:28px;border-radius:50%;display:inline-flex;align-items:center;justify-content:center;font-size:11px;font-weight:700;margin-right:8px;flex-shrink:0;}
  .user-info{display:flex;flex-direction:column;}
  .user-name{font-weight:600;font-size:13px;}
  .user-id{font-size:10px;color:var(--text-dim);font-family:'Space Mono',monospace;}
  .chip{display:inline-flex;align-items:center;padding:3px 8px;border-radius:20px;font-size:10px;font-weight:700;font-family:'Space Mono',monospace;}
  .chip-green{background:rgba(0,229,160,0.1);color:var(--accent);border:1px solid rgba(0,229,160,0.2);}
  .chip-red{background:rgba(255,107,107,0.1);color:var(--accent3);border:1px solid rgba(255,107,107,0.2);}
  .chip-yellow{background:rgba(255,209,102,0.1);color:var(--accent4);border:1px solid rgba(255,209,102,0.2);}
  .chip-purple{background:rgba(124,106,247,0.1);color:var(--accent2);border:1px solid rgba(124,106,247,0.2);}
  .action-btns{display:flex;gap:6px;}
  .icon-btn{width:28px;height:28px;border-radius:6px;border:1px solid var(--border);background:transparent;color:var(--text-dim);font-size:13px;cursor:pointer;display:flex;align-items:center;justify-content:center;transition:all 0.15s;}
  .icon-btn:hover{background:var(--surface2);color:var(--text);}
  .icon-btn.danger:hover{background:rgba(255,107,107,0.1);color:var(--accent3);border-color:rgba(255,107,107,0.3);}

  /* FORM */
  input[type="text"],input[type="number"],input[type="password"],textarea,select{
    background:var(--surface2);border:1px solid var(--border);border-radius:8px;
    color:var(--text);font-family:'Syne',sans-serif;font-size:13px;outline:none;transition:border-color 0.15s;
  }
  input[type="text"]:focus,input[type="number"]:focus,input[type="password"]:focus,textarea:focus,select:focus{border-color:var(--accent);}
  select{padding:9px 12px;cursor:pointer;}
  select option{background:var(--surface2);}
  .form-group{margin-bottom:18px;}
  .form-label{display:block;font-size:10px;font-weight:700;text-transform:uppercase;letter-spacing:1px;color:var(--text-dim);margin-bottom:7px;font-family:'Space Mono',monospace;}
  textarea{width:100%;padding:12px;border-radius:8px;resize:vertical;min-height:90px;font-size:13px;line-height:1.6;}

  /* CMD */
  .cmd-list{display:flex;flex-direction:column;gap:10px;}
  .cmd-item{background:var(--surface2);border:1px solid var(--border);border-radius:10px;padding:14px 16px;display:flex;align-items:center;gap:14px;transition:border-color 0.15s;}
  .cmd-item:hover{border-color:var(--text-dim);}
  .cmd-slug{font-family:'Space Mono',monospace;font-size:13px;color:var(--accent);min-width:120px;}
  .cmd-desc{font-size:12px;color:var(--text-dim);flex:1;}

  /* SETTINGS */
  .settings-grid{display:grid;grid-template-columns:1fr 1fr;gap:20px;}
  .setting-row{display:flex;align-items:center;justify-content:space-between;padding:14px 0;border-bottom:1px solid var(--border);}
  .setting-row:last-child{border-bottom:none;}
  .setting-name{font-size:13px;font-weight:600;}
  .setting-desc{font-size:11px;color:var(--text-dim);margin-top:2px;}
  .toggle{width:42px;height:24px;background:var(--surface2);border:1px solid var(--border);border-radius:12px;cursor:pointer;position:relative;transition:all 0.2s;flex-shrink:0;}
  .toggle.on{background:var(--accent);border-color:var(--accent);}
  .toggle::after{content:'';position:absolute;width:16px;height:16px;border-radius:50%;background:#fff;top:3px;left:3px;transition:left 0.2s;}
  .toggle.on::after{left:21px;}

  /* LOGS */
  .log-terminal{background:#050508;border:1px solid var(--border);border-radius:12px;padding:20px;font-family:'Space Mono',monospace;font-size:11px;height:360px;overflow-y:auto;line-height:1.9;}
  .log-line{display:flex;gap:12px;flex-wrap:wrap;}
  .log-time{color:var(--text-muted);flex-shrink:0;}
  .log-info{color:#58a6ff;}
  .log-warn{color:var(--accent4);}
  .log-error{color:var(--accent3);}
  .log-success{color:var(--accent);}

  /* PROGRESS */
  .progress-bar-wrap{height:6px;background:var(--surface2);border-radius:3px;overflow:hidden;margin-top:8px;}
  .progress-bar{height:100%;background:linear-gradient(90deg,var(--accent),var(--accent2));border-radius:3px;transition:width 0.3s;}

  /* MODAL */
  .modal-overlay{display:none;position:fixed;inset:0;background:rgba(0,0,0,0.7);backdrop-filter:blur(4px);z-index:100;align-items:center;justify-content:center;}
  .modal-overlay.open{display:flex;}
  .modal{background:var(--surface);border:1px solid var(--border);border-radius:16px;padding:28px;width:440px;position:relative;animation:modalIn 0.2s ease;}
  @keyframes modalIn{from{opacity:0;transform:scale(0.95)}to{opacity:1;transform:none}}
  .modal-title{font-size:16px;font-weight:800;margin-bottom:20px;}
  .modal-close{position:absolute;top:20px;right:20px;background:none;border:none;color:var(--text-dim);font-size:18px;cursor:pointer;}
  .modal-close:hover{color:var(--text);}
  .modal-actions{display:flex;gap:10px;justify-content:flex-end;margin-top:20px;}

  /* TOAST */
  .toast{position:fixed;bottom:28px;right:28px;background:var(--surface);border:1px solid var(--border);border-radius:10px;padding:14px 18px;display:flex;align-items:center;gap:10px;font-size:13px;font-weight:600;z-index:200;transform:translateY(80px);opacity:0;transition:all 0.3s ease;min-width:260px;}
  .toast.show{transform:none;opacity:1;}
  .toast.success{border-left:3px solid var(--accent);}
  .toast.error{border-left:3px solid var(--accent3);}

  /* LOADING */
  .loading{display:inline-block;width:14px;height:14px;border:2px solid rgba(0,229,160,0.3);border-top-color:var(--accent);border-radius:50%;animation:spin 0.7s linear infinite;vertical-align:middle;}
  @keyframes spin{to{transform:rotate(360deg)}}

  .grid-2{display:grid;grid-template-columns:1fr 1fr;gap:20px;}
  .mt-16{margin-top:16px;}
  .mt-24{margin-top:24px;}
  .w-full{width:100%;}
  .api-status{display:flex;align-items:center;gap:6px;font-size:11px;font-family:'Space Mono',monospace;color:var(--text-dim);}
</style>
</head>
<body>

<!-- ═══ LOGIN SCREEN ═══ -->
<div id="login-screen">
  <div class="login-box">
    <div class="login-logo">
      <div class="login-logo-icon">🤖</div>
      <div>
        <div style="font-size:22px;font-weight:800;">BotPanel</div>
        <div style="font-size:11px;color:var(--text-dim);font-family:'Space Mono',monospace;">Telegram Bot 控制台</div>
      </div>
    </div>
    <div class="login-title">连接你的 Bot</div>
    <div class="login-desc">输入 Bot Token 连接并管理你的 Telegram Bot。Token 仅保存在浏览器内存，关闭页面即清除，不会上传任何服务器。</div>
    <div id="login-error" class="login-error"></div>
    <div class="login-input-wrap">
      <input type="password" class="login-input" id="token-input"
        placeholder="123456789:AAxxxxxxxxxxxxxxxxxxxxxxxx"
        onkeydown="if(event.key==='Enter')doLogin()">
      <span class="login-eye" onclick="toggleTokenVis()" id="eye-btn">👁</span>
    </div>
    <div class="login-hint">从 <b>@BotFather</b> → /mybots → 选择 Bot → API Token</div>
    <button class="login-btn" id="login-btn" onclick="doLogin()">🔗 连接 Bot</button>
    <div class="login-security">
      <span style="font-size:20px;flex-shrink:0;">🔒</span>
      <div class="login-security-text"><b>完全本地</b>：Token 只存于页面内存，不记录、不传输、不持久化。刷新页面需重新输入。</div>
    </div>
  </div>
</div>

<!-- ═══ SIDEBAR ═══ -->
<aside class="sidebar" id="app-sidebar" style="display:none;">
  <div class="logo">
    <div class="logo-icon">🤖</div>
    <div>
      <div class="logo-text">BotPanel</div>
      <div class="logo-sub">v2.4.1</div>
    </div>
  </div>
  <nav>
    <div class="nav-label">主菜单</div>
    <div class="nav-section">
      <div class="nav-item active" onclick="goto('dashboard',this)"><span class="nav-icon">📊</span>数据总览</div>
      <div class="nav-item" onclick="goto('users',this)"><span class="nav-icon">👥</span>用户 & 消息</div>
      <div class="nav-item" onclick="goto('broadcast',this)"><span class="nav-icon">📢</span>消息广播<span class="badge" id="bc-badge" style="display:none;"></span></div>
    </div>
    <div class="nav-label">配置</div>
    <div class="nav-section">
      <div class="nav-item" onclick="goto('commands',this)"><span class="nav-icon">⌨️</span>命令管理<span class="badge" id="cmd-badge">0</span></div>
      <div class="nav-item" onclick="goto('settings',this)"><span class="nav-icon">⚙️</span>Bot 设置</div>
      <div class="nav-item" onclick="goto('logs',this)"><span class="nav-icon">📋</span>运行日志</div>
    </div>
  </nav>
  <div class="bot-status">
    <div class="bot-status-header">
      <div class="status-dot"></div>
      <span class="status-label">在线运行中</span>
    </div>
    <div class="bot-name" id="sidebar-botname">@loading...</div>
    <div class="bot-token-display" id="sidebar-token">token: ****</div>
  </div>
  <button class="logout-btn" onclick="doLogout()">🚪 断开连接</button>
</aside>

<!-- ═══ MAIN ═══ -->
<div class="main" id="app-main" style="display:none;">
  <div class="topbar">
    <div class="page-title" id="page-title">数据总览</div>
    <div class="topbar-actions">
      <div class="api-status"><span style="color:var(--accent);">●</span>&nbsp;已连接</div>
      <button class="btn btn-ghost" onclick="refreshCurrent()">🔄 刷新</button>
      <button class="btn btn-primary" onclick="openModal('broadcast-quick')">+ 广播</button>
    </div>
  </div>
  <div class="content">

    <!-- ── Dashboard ── -->
    <div class="page active" id="page-dashboard">
      <div class="stats-grid">
        <div class="stat-card green"><div class="stat-icon">🤖</div><div class="stat-value green" id="stat-name" style="font-size:16px;">–</div><div class="stat-label">Bot 名称</div><div class="stat-change" id="stat-id">–</div></div>
        <div class="stat-card purple"><div class="stat-icon">👥</div><div class="stat-value purple">实时</div><div class="stat-label">getUpdates 模式</div><div class="stat-change" id="stat-updates-count">–</div></div>
        <div class="stat-card yellow"><div class="stat-icon">🔗</div><div class="stat-value yellow" id="stat-webhook-status" style="font-size:14px;">–</div><div class="stat-label">Webhook 状态</div><div class="stat-change" id="stat-pending">–</div></div>
        <div class="stat-card red"><div class="stat-icon">⚡</div><div class="stat-value red" id="stat-ping">–</div><div class="stat-label">API 延迟 (ms)</div><div class="stat-change">Telegram API</div></div>
      </div>
      <div class="charts-row">
        <div class="card">
          <div class="card-header"><div><div class="card-title">📋 Bot 详细信息</div><div class="card-subtitle">来自 getMe API 实时数据</div></div></div>
          <div class="card-body">
            <div id="bot-info-grid" style="display:grid;grid-template-columns:1fr 1fr;gap:10px;font-size:12px;"></div>
          </div>
        </div>
        <div class="card">
          <div class="card-header"><div class="card-title">⌨️ 已注册命令</div><button class="btn btn-ghost" style="font-size:11px;padding:5px 10px;" onclick="goto('commands',null)">管理</button></div>
          <div class="card-body" style="padding:14px 16px;"><div id="cmd-quick-list" style="display:flex;flex-direction:column;gap:6px;font-size:12px;color:var(--text-dim);">加载中...</div></div>
        </div>
      </div>
      <div class="card">
        <div class="card-header">
          <div><div class="card-title">🔔 最近消息 (getUpdates)</div><div class="card-subtitle">实时拉取，Webhook 模式下可能为空</div></div>
          <button class="btn btn-ghost" style="font-size:11px;padding:5px 10px;" onclick="loadUpdates()">🔄 刷新</button>
        </div>
        <div class="table-wrap">
          <table>
            <thead><tr><th>Update ID</th><th>用户</th><th>内容</th><th>时间</th><th>类型</th></tr></thead>
            <tbody id="updates-tbody"><tr><td colspan="5" style="text-align:center;padding:24px;color:var(--text-dim);font-size:12px;"><span class="loading"></span> 加载中...</td></tr></tbody>
          </table>
        </div>
      </div>
    </div>

    <!-- ── Users ── -->
    <div class="page" id="page-users">
      <div class="grid-2" style="margin-bottom:20px;">
        <div class="card">
          <div class="card-header"><div class="card-title">🔍 查询用户 / 聊天</div></div>
          <div class="card-body">
            <div class="form-group">
              <label class="form-label">Chat ID 或 @用户名</label>
              <div style="display:flex;gap:8px;">
                <input type="text" id="user-query-input" placeholder="@username 或 123456789" style="flex:1;padding:9px 12px;">
                <button class="btn btn-primary" onclick="lookupUser()">查询</button>
              </div>
            </div>
            <div id="user-result" style="display:none;background:var(--surface2);border-radius:10px;padding:14px;font-size:12px;line-height:1.8;"></div>
          </div>
        </div>
        <div class="card">
          <div class="card-header"><div class="card-title">✉️ 发送私信</div></div>
          <div class="card-body">
            <div class="form-group">
              <label class="form-label">Chat ID</label>
              <input type="text" id="send-chat-id" placeholder="@username 或 123456789" style="width:100%;padding:9px 12px;">
            </div>
            <div class="form-group">
              <label class="form-label">消息内容</label>
              <textarea id="send-msg-content" placeholder="消息内容... 支持 Markdown" style="min-height:70px;"></textarea>
            </div>
            <div style="display:flex;gap:8px;">
              <select id="send-parse-mode" style="flex:1;">
                <option value="">纯文本</option>
                <option value="Markdown">Markdown</option>
                <option value="HTML">HTML</option>
              </select>
              <button class="btn btn-primary" onclick="sendMessageToUser()">📤 发送</button>
            </div>
          </div>
        </div>
      </div>
      <div class="card">
        <div class="card-header"><div class="card-title">📨 发送其他类型消息</div></div>
        <div class="card-body">
          <div style="display:grid;grid-template-columns:repeat(3,1fr);gap:12px;">
            <div>
              <label class="form-label">Chat ID</label>
              <input type="text" id="adv-chat-id" placeholder="Chat ID" style="width:100%;padding:9px 12px;margin-bottom:8px;">
            </div>
            <div>
              <label class="form-label">图片 URL（sendPhoto）</label>
              <input type="text" id="adv-photo" placeholder="https://..." style="width:100%;padding:9px 12px;margin-bottom:8px;">
            </div>
            <div style="display:flex;align-items:flex-end;">
              <button class="btn btn-ghost w-full" onclick="sendPhoto()">📸 发送图片</button>
            </div>
          </div>
          <div style="margin-top:10px;display:grid;grid-template-columns:1fr 1fr;gap:12px;">
            <div>
              <label class="form-label">转发来源 Chat ID</label>
              <input type="text" id="fwd-from" placeholder="来源 Chat ID" style="width:100%;padding:9px 12px;">
            </div>
            <div>
              <label class="form-label">转发消息 ID</label>
              <div style="display:flex;gap:8px;">
                <input type="number" id="fwd-msg-id" placeholder="消息 ID" style="flex:1;padding:9px 12px;">
                <button class="btn btn-ghost" onclick="forwardMsg()">↩️ 转发</button>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>

    <!-- ── Broadcast ── -->
    <div class="page" id="page-broadcast">
      <div class="grid-2">
        <div>
          <div class="card">
            <div class="card-header"><div class="card-title">📢 批量广播消息</div></div>
            <div class="card-body">
              <div class="form-group">
                <label class="form-label">目标 Chat ID 列表（每行一个）</label>
                <textarea id="bc-targets" placeholder="123456789&#10;987654321&#10;@channelname" style="min-height:80px;font-family:'Space Mono';font-size:11px;"></textarea>
                <div style="font-size:10px;color:var(--text-dim);margin-top:5px;">支持用户ID / 群组ID / 频道用户名，每行一个</div>
              </div>
              <div class="form-group">
                <label class="form-label">消息内容</label>
                <textarea id="bc-msg" placeholder="输入广播内容..."></textarea>
              </div>
              <div style="display:grid;grid-template-columns:1fr 1fr;gap:10px;" class="form-group">
                <div>
                  <label class="form-label">解析模式</label>
                  <select id="bc-parse" style="width:100%;">
                    <option value="">纯文本</option>
                    <option value="Markdown">Markdown</option>
                    <option value="HTML">HTML</option>
                  </select>
                </div>
                <div>
                  <label class="form-label">间隔延迟 (ms)</label>
                  <input type="number" id="bc-delay" value="500" min="100" max="10000" style="width:100%;padding:9px 12px;">
                </div>
              </div>
              <button class="btn btn-primary w-full" id="bc-btn" onclick="startBroadcast()">🚀 开始广播</button>
              <div id="bc-progress" style="margin-top:14px;display:none;">
                <div style="display:flex;justify-content:space-between;font-size:11px;color:var(--text-dim);margin-bottom:4px;">
                  <span>广播进度</span><span id="bc-progress-text">0 / 0</span>
                </div>
                <div class="progress-bar-wrap"><div class="progress-bar" id="bc-bar" style="width:0%"></div></div>
                <div id="bc-result-log" style="margin-top:10px;max-height:100px;overflow-y:auto;font-size:10px;font-family:'Space Mono',monospace;color:var(--text-dim);line-height:1.7;"></div>
              </div>
            </div>
          </div>
        </div>
        <div>
          <div class="card" style="margin-bottom:16px;">
            <div class="card-header"><div class="card-title">📊 广播历史</div></div>
            <div class="card-body" id="bc-history" style="font-size:12px;color:var(--text-dim);min-height:60px;">暂无记录</div>
          </div>
          <div class="card">
            <div class="card-header"><div class="card-title">💡 注意事项</div></div>
            <div class="card-body" style="font-size:12px;color:var(--text-dim);line-height:2;">
              <div>• 用户必须先 /start 过 Bot 才能收到消息</div>
              <div>• 建议延迟 ≥ 500ms，避免触发 API 限流</div>
              <div>• 群组/频道需要 Bot 有发消息权限</div>
              <div>• Markdown: <code style="background:var(--surface2);padding:1px 4px;border-radius:3px;">*粗体* _斜体_ `代码`</code></div>
            </div>
          </div>
        </div>
      </div>
    </div>

    <!-- ── Commands ── -->
    <div class="page" id="page-commands">
      <div style="display:flex;justify-content:space-between;align-items:center;margin-bottom:20px;">
        <div><div style="font-size:13px;font-weight:700;">Bot 命令管理</div><div style="font-size:11px;color:var(--text-dim);margin-top:2px;">通过 setMyCommands API 实时同步</div></div>
        <div style="display:flex;gap:10px;">
          <button class="btn btn-ghost" onclick="loadCommands()">🔄 刷新</button>
          <button class="btn btn-danger" onclick="deleteAllCommands()">🗑 清除全部</button>
          <button class="btn btn-primary" onclick="openModal('add-cmd')">+ 添加命令</button>
        </div>
      </div>
      <div class="cmd-list" id="cmd-list-container">
        <div style="text-align:center;padding:30px;color:var(--text-dim);font-size:13px;"><span class="loading"></span> 加载中...</div>
      </div>
    </div>

    <!-- ── Settings ── -->
    <div class="page" id="page-settings">
      <div class="settings-grid">
        <div class="card">
          <div class="card-header"><div class="card-title">🔗 Webhook 管理</div></div>
          <div class="card-body">
            <div class="form-group">
              <label class="form-label">当前 Webhook 状态</label>
              <div id="webhook-info" style="background:var(--surface2);border-radius:8px;padding:12px;font-size:11px;font-family:'Space Mono',monospace;line-height:1.8;min-height:60px;">加载中...</div>
            </div>
            <div class="form-group">
              <label class="form-label">设置新 Webhook URL</label>
              <input type="text" id="webhook-url" placeholder="https://yourserver.com/webhook/token" style="width:100%;padding:9px 12px;">
            </div>
            <div style="display:flex;gap:10px;">
              <button class="btn btn-primary" style="flex:1;" onclick="setWebhook()">✅ 设置</button>
              <button class="btn btn-danger" style="flex:1;" onclick="deleteWebhook()">🗑 删除</button>
            </div>
          </div>
        </div>
        <div class="card">
          <div class="card-header"><div class="card-title">🔑 Token 管理</div></div>
          <div class="card-body">
            <div class="form-group">
              <label class="form-label">当前 Token</label>
              <div style="display:flex;gap:8px;">
                <input type="password" id="current-token-display" style="flex:1;padding:9px 12px;" readonly>
                <button class="btn btn-ghost" onclick="toggleCurrentToken()">👁</button>
                <button class="btn btn-ghost" onclick="copyToken()">📋</button>
              </div>
            </div>
            <div class="form-group">
              <label class="form-label">切换到新 Token</label>
              <input type="text" id="new-token-input" placeholder="新的 Bot Token" style="width:100%;padding:9px 12px;">
            </div>
            <div style="display:flex;gap:10px;">
              <button class="btn btn-primary" style="flex:1;" onclick="switchToken()">🔄 切换</button>
              <button class="btn btn-ghost" style="flex:1;" onclick="testConnection()">🏓 测试连接</button>
            </div>
          </div>
        </div>
      </div>
      <div class="card mt-16">
        <div class="card-header"><div class="card-title">📄 getMe 原始响应</div></div>
        <div class="card-body"><pre id="getme-raw" style="font-size:11px;font-family:'Space Mono',monospace;color:var(--text-dim);line-height:1.7;white-space:pre-wrap;word-break:break-all;">加载中...</pre></div>
      </div>
    </div>

    <!-- ── Logs ── -->
    <div class="page" id="page-logs">
      <div style="display:flex;gap:10px;margin-bottom:16px;align-items:center;">
        <select id="log-filter" onchange="renderLogs()" style="padding:9px 12px;font-size:12px;">
          <option>全部级别</option><option>INFO</option><option>WARN</option><option>ERROR</option>
        </select>
        <input type="text" placeholder="搜索日志..." id="log-search" style="flex:1;padding:9px 12px;" oninput="renderLogs()">
        <button class="btn btn-ghost" onclick="clearLogs()">🗑 清空</button>
        <button class="btn btn-ghost" onclick="exportLogs()">📥 导出</button>
        <button class="btn btn-primary" onclick="loadUpdates()">🔄 拉取更新</button>
      </div>
      <div class="log-terminal" id="log-terminal"></div>
    </div>

  </div>
</div>

<!-- ═══ MODALS ═══ -->
<div class="modal-overlay" id="modal-add-cmd">
  <div class="modal">
    <button class="modal-close" onclick="closeModal('add-cmd')">✕</button>
    <div class="modal-title">➕ 添加命令</div>
    <div id="add-cmd-error" style="background:rgba(255,107,107,0.1);border:1px solid rgba(255,107,107,0.3);border-radius:8px;padding:10px;font-size:12px;color:var(--accent3);margin-bottom:14px;display:none;"></div>
    <div class="form-group">
      <label class="form-label">命令名（不含 /）</label>
      <input type="text" id="new-cmd-name" placeholder="start" style="width:100%;padding:9px 12px;">
    </div>
    <div class="form-group">
      <label class="form-label">命令描述（用户可见）</label>
      <input type="text" id="new-cmd-desc" placeholder="开始使用 Bot" style="width:100%;padding:9px 12px;">
    </div>
    <div style="font-size:11px;color:var(--text-muted);margin-top:-10px;margin-bottom:4px;">命令描述显示在 / 菜单里，实际响应逻辑需要在你的后端代码里实现。</div>
    <div class="modal-actions">
      <button class="btn btn-ghost" onclick="closeModal('add-cmd')">取消</button>
      <button class="btn btn-primary" onclick="addCommand()">确认添加</button>
    </div>
  </div>
</div>

<div class="modal-overlay" id="modal-broadcast-quick">
  <div class="modal">
    <button class="modal-close" onclick="closeModal('broadcast-quick')">✕</button>
    <div class="modal-title">📢 快速发送</div>
    <div class="form-group">
      <label class="form-label">目标 Chat ID（逗号分隔）</label>
      <input type="text" id="quick-targets" placeholder="123456789, @channel" style="width:100%;padding:9px 12px;">
    </div>
    <div class="form-group">
      <label class="form-label">消息内容</label>
      <textarea id="quick-msg" placeholder="消息内容..."></textarea>
    </div>
    <div class="modal-actions">
      <button class="btn btn-ghost" onclick="closeModal('broadcast-quick')">取消</button>
      <button class="btn btn-primary" onclick="quickBroadcast()">🚀 发送</button>
    </div>
  </div>
</div>

<!-- Toast -->
<div class="toast" id="toast"><span id="toast-icon">✓</span><span id="toast-msg"></span></div>

<script>
// ═══ STATE ═══
let BOT_TOKEN = '';
let botInfo = null;
let logEntries = [];
let currentPage = 'dashboard';
let bcHistory = [];

// ═══ API HELPER ═══
const TG = (method, params={}) =>
  fetch(`https://api.telegram.org/bot${BOT_TOKEN}/${method}`, {
    method:'POST', headers:{'Content-Type':'application/json'}, body:JSON.stringify(params)
  }).then(r=>r.json());

// ═══ LOGIN ═══
function toggleTokenVis(){
  const i=document.getElementById('token-input'),e=document.getElementById('eye-btn');
  i.type=i.type==='password'?'text':'password'; e.textContent=i.type==='password'?'👁':'🙈';
}

async function doLogin(){
  const token=document.getElementById('token-input').value.trim();
  if(!token){showLoginErr('请输入 Token');return;}
  const btn=document.getElementById('login-btn');
  btn.disabled=true; btn.innerHTML='<span class="loading"></span> 验证中...';
  document.getElementById('login-error').style.display='none';
  const t0=Date.now();
  BOT_TOKEN=token;
  try{
    const res=await TG('getMe');
    if(!res.ok) throw new Error(res.description||'Token 无效');
    const ping=Date.now()-t0;
    botInfo=res.result;
    addLog('INFO',`登录成功: @${botInfo.username} (ID:${botInfo.id}) | 延迟 ${ping}ms`);
    document.getElementById('login-screen').style.display='none';
    document.getElementById('app-sidebar').style.display='flex';
    document.getElementById('app-main').style.display='flex';
    document.getElementById('sidebar-botname').textContent='@'+botInfo.username;
    document.getElementById('sidebar-token').textContent='token: '+token.substring(0,8)+'...';
    document.getElementById('current-token-display').value=token;
    document.getElementById('getme-raw').textContent=JSON.stringify(botInfo,null,2);
    loadDashboard(ping); loadCommands(); loadWebhookInfo();
  }catch(e){
    BOT_TOKEN='';
    showLoginErr('❌ '+e.message);
    btn.disabled=false; btn.textContent='🔗 连接 Bot';
  }
}

function showLoginErr(msg){
  const el=document.getElementById('login-error');
  el.textContent=msg; el.style.display='block';
}

function doLogout(){
  BOT_TOKEN=''; botInfo=null; logEntries=[]; bcHistory=[];
  ['login-screen'].forEach(id=>document.getElementById(id).style.display='flex');
  ['app-sidebar','app-main'].forEach(id=>document.getElementById(id).style.display='none');
  document.getElementById('token-input').value='';
  document.getElementById('login-error').style.display='none';
  document.getElementById('login-btn').disabled=false;
  document.getElementById('login-btn').textContent='🔗 连接 Bot';
}

// ═══ NAV ═══
const pageNames={dashboard:'数据总览',users:'用户 & 消息',broadcast:'消息广播',commands:'命令管理',settings:'Bot 设置',logs:'运行日志'};
function goto(page,el){
  document.querySelectorAll('.page').forEach(p=>p.classList.remove('active'));
  document.querySelectorAll('.nav-item').forEach(n=>n.classList.remove('active'));
  document.getElementById('page-'+page).classList.add('active');
  document.getElementById('page-title').textContent=pageNames[page];
  if(el) el.classList.add('active');
  currentPage=page;
  if(page==='logs') renderLogs();
  if(page==='settings') loadWebhookInfo();
  if(page==='commands') loadCommands();
}

function refreshCurrent(){
  if(currentPage==='dashboard') loadDashboard();
  else if(currentPage==='commands') loadCommands();
  else if(currentPage==='settings') loadWebhookInfo();
  else if(currentPage==='logs') loadUpdates();
  else showToast('已刷新','success');
}

// ═══ DASHBOARD ═══
async function loadDashboard(ping){
  if(!ping){const t0=Date.now();await TG('getMe');ping=Date.now()-t0;}
  document.getElementById('stat-name').textContent=botInfo.first_name;
  document.getElementById('stat-id').textContent='ID: '+botInfo.id+' | @'+botInfo.username;
  document.getElementById('stat-ping').textContent=ping;

  // bot info grid
  const grid=document.getElementById('bot-info-grid');
  const rows=[
    ['Bot ID', botInfo.id],
    ['用户名', '@'+botInfo.username],
    ['显示名', botInfo.first_name+(botInfo.last_name?' '+botInfo.last_name:'')],
    ['内联支持', botInfo.supports_inline_queries?'✅ 支持':'❌ 不支持'],
    ['可加群组', botInfo.can_join_groups?'✅ 是':'❌ 否'],
    ['读群消息', botInfo.can_read_all_group_messages?'✅ 可以':'⚠️ 隐私模式'],
  ];
  grid.innerHTML=rows.map(([k,v])=>`
    <div style="background:var(--surface2);border-radius:8px;padding:10px 12px;">
      <div style="font-size:10px;color:var(--text-muted);font-family:'Space Mono';margin-bottom:3px;">${k}</div>
      <div style="font-size:12px;font-weight:600;">${v}</div>
    </div>`).join('');

  // Webhook
  const wh=await TG('getWebhookInfo');
  if(wh.ok){
    const w=wh.result;
    document.getElementById('stat-webhook-status').textContent=w.url?'Webhook':'轮询';
    document.getElementById('stat-pending').textContent='待处理: '+(w.pending_update_count??0);
  }

  await loadUpdates();

  // Commands quick
  const cmds=await TG('getMyCommands');
  const ql=document.getElementById('cmd-quick-list');
  if(cmds.ok&&cmds.result.length>0){
    ql.innerHTML=cmds.result.map(c=>`
      <div style="display:flex;gap:8px;padding:5px 0;border-bottom:1px solid var(--border);">
        <span style="font-family:'Space Mono';font-size:11px;color:var(--accent);min-width:80px;">/${c.command}</span>
        <span style="font-size:11px;color:var(--text-dim);">${c.description}</span>
      </div>`).join('');
  } else {
    ql.innerHTML='<div style="color:var(--text-muted);font-size:12px;">暂无命令</div>';
  }
}

async function loadUpdates(){
  addLog('INFO','正在拉取 getUpdates...');
  try{
    const res=await TG('getUpdates',{limit:20,timeout:0});
    if(!res.ok){addLog('ERROR','getUpdates 失败: '+res.description);return;}
    const updates=res.result;
    document.getElementById('stat-updates-count').textContent=`已获取 ${updates.length} 条`;
    const tbody=document.getElementById('updates-tbody');
    if(!updates.length){
      tbody.innerHTML='<tr><td colspan="5" style="text-align:center;padding:24px;color:var(--text-dim);font-size:12px;">暂无新消息（可能使用 Webhook 模式）</td></tr>';
      addLog('INFO','暂无新更新'); return;
    }
    tbody.innerHTML=updates.map(u=>{
      const msg=u.message||u.edited_message||u.channel_post||u.callback_query?.message;
      const from=u.message?.from||u.edited_message?.from||u.callback_query?.from;
      const text=(u.message?.text||u.edited_message?.text||u.callback_query?.data||u.channel_post?.text||'[非文本]');
      const time=msg?.date?new Date(msg.date*1000).toLocaleTimeString('zh-CN',{hour12:false}):'–';
      const type=u.callback_query?'回调':u.edited_message?'编辑':u.channel_post?'频道':'消息';
      const uname=from?(from.username?'@'+from.username:from.first_name):(msg?.chat?.title||'–');
      const uid=from?.id||msg?.chat?.id||'–';
      const avatar=(uname[1]||uname[0]||'?').toUpperCase();
      return `<tr>
        <td style="font-family:'Space Mono';font-size:10px;color:var(--text-muted);">${u.update_id}</td>
        <td><div class="user-cell">
          <div class="user-avatar" style="background:linear-gradient(135deg,var(--accent),var(--accent2));color:#0a0a0f;font-size:10px;width:26px;height:26px;">${avatar}</div>
          <div class="user-info"><span class="user-name" style="font-size:12px;">${uname}</span><span class="user-id">${uid}</span></div>
        </div></td>
        <td style="font-size:11px;max-width:180px;overflow:hidden;text-overflow:ellipsis;white-space:nowrap;" title="${text.replace(/"/g,'')}">${text.substring(0,50)}${text.length>50?'...':''}</td>
        <td style="font-size:10px;color:var(--text-dim);font-family:'Space Mono';">${time}</td>
        <td><span class="chip chip-purple" style="font-size:9px;">${type}</span></td>
      </tr>`;
    }).join('');
    addLog('INFO',`加载了 ${updates.length} 条更新`);
  }catch(e){addLog('ERROR','loadUpdates 异常: '+e.message);}
}

// ═══ USERS ═══
async function lookupUser(){
  const id=document.getElementById('user-query-input').value.trim();
  if(!id){showToast('请输入 Chat ID','error');return;}
  const res=await TG('getChat',{chat_id:id});
  const el=document.getElementById('user-result');
  el.style.display='block';
  if(!res.ok){el.innerHTML=`<span style="color:var(--accent3);">❌ ${res.description}</span>`;addLog('ERROR','查询失败: '+res.description);return;}
  const c=res.result;
  el.innerHTML=`
    <div style="display:grid;grid-template-columns:1fr 1fr;gap:8px;">
      <div><span style="color:var(--text-dim);font-size:10px;font-family:'Space Mono';">ID</span><div style="font-family:'Space Mono';font-size:12px;">${c.id}</div></div>
      <div><span style="color:var(--text-dim);font-size:10px;font-family:'Space Mono';">类型</span><div style="font-size:12px;">${c.type}</div></div>
      <div><span style="color:var(--text-dim);font-size:10px;font-family:'Space Mono';">名称</span><div style="font-size:12px;">${c.first_name||''} ${c.last_name||''} ${c.title||''}</div></div>
      <div><span style="color:var(--text-dim);font-size:10px;font-family:'Space Mono';">用户名</span><div style="font-family:'Space Mono';font-size:12px;">${c.username?'@'+c.username:'–'}</div></div>
    </div>
    ${c.bio?`<div style="margin-top:8px;font-size:11px;color:var(--text-dim);">简介: ${c.bio}</div>`:''}`;
  addLog('INFO',`查询: ${c.first_name||c.title} (${c.id})`);
  showToast('查询成功','success');
}

async function sendMessageToUser(){
  const chat_id=document.getElementById('send-chat-id').value.trim();
  const text=document.getElementById('send-msg-content').value.trim();
  const parse_mode=document.getElementById('send-parse-mode').value;
  if(!chat_id||!text){showToast('请填写完整信息','error');return;}
  const params={chat_id,text};
  if(parse_mode) params.parse_mode=parse_mode;
  const res=await TG('sendMessage',params);
  if(res.ok){showToast('✅ 发送成功','success');addLog('INFO',`发送消息到 ${chat_id}`);}
  else{showToast('❌ '+res.description,'error');addLog('ERROR','发送失败: '+res.description);}
}

async function sendPhoto(){
  const chat_id=document.getElementById('adv-chat-id').value.trim();
  const photo=document.getElementById('adv-photo').value.trim();
  if(!chat_id||!photo){showToast('请填写 Chat ID 和图片 URL','error');return;}
  const res=await TG('sendPhoto',{chat_id,photo});
  if(res.ok){showToast('📸 图片发送成功','success');addLog('INFO',`发送图片到 ${chat_id}`);}
  else{showToast('❌ '+res.description,'error');addLog('ERROR','发送图片失败: '+res.description);}
}

async function forwardMsg(){
  const chat_id=document.getElementById('adv-chat-id').value.trim();
  const from_chat_id=document.getElementById('fwd-from').value.trim();
  const message_id=parseInt(document.getElementById('fwd-msg-id').value);
  if(!chat_id||!from_chat_id||!message_id){showToast('请填写完整的转发信息','error');return;}
  const res=await TG('forwardMessage',{chat_id,from_chat_id,message_id});
  if(res.ok){showToast('↩️ 转发成功','success');addLog('INFO',`转发消息 ${message_id} 到 ${chat_id}`);}
  else{showToast('❌ '+res.description,'error');addLog('ERROR','转发失败: '+res.description);}
}

// ═══ BROADCAST ═══
async function startBroadcast(){
  const rawTargets=document.getElementById('bc-targets').value.trim();
  const text=document.getElementById('bc-msg').value.trim();
  const parse_mode=document.getElementById('bc-parse').value;
  const delay=parseInt(document.getElementById('bc-delay').value)||500;
  if(!rawTargets||!text){showToast('请填写目标和消息','error');return;}
  const targets=rawTargets.split('\n').map(t=>t.trim()).filter(Boolean);
  if(!targets.length){showToast('目标列表为空','error');return;}
  const btn=document.getElementById('bc-btn');
  btn.disabled=true; btn.textContent='广播中...';
  const prog=document.getElementById('bc-progress');
  const bar=document.getElementById('bc-bar');
  const progText=document.getElementById('bc-progress-text');
  const resultLog=document.getElementById('bc-result-log');
  prog.style.display='block'; resultLog.innerHTML='';
  let success=0,fail=0;
  for(let i=0;i<targets.length;i++){
    const t=targets[i];
    bar.style.width=Math.round((i+1)/targets.length*100)+'%';
    progText.textContent=`${i+1} / ${targets.length}`;
    try{
      const params={chat_id:t,text};
      if(parse_mode) params.parse_mode=parse_mode;
      const res=await TG('sendMessage',params);
      if(res.ok){success++;resultLog.innerHTML+=`<div style="color:var(--accent)">✓ ${t}</div>`;addLog('INFO',`广播→${t}: 成功`);}
      else{fail++;resultLog.innerHTML+=`<div style="color:var(--accent3)">✗ ${t}: ${res.description}</div>`;addLog('ERROR',`广播→${t}: ${res.description}`);}
    }catch(e){fail++;resultLog.innerHTML+=`<div style="color:var(--accent3)">✗ ${t}: ${e.message}</div>`;}
    resultLog.scrollTop=resultLog.scrollHeight;
    if(i<targets.length-1) await sleep(delay);
  }
  bcHistory.unshift({time:new Date().toLocaleString('zh-CN'),total:targets.length,success,fail,text:text.substring(0,25)+'...'});
  renderBcHistory();
  showToast(`广播完成 ✓${success} ✗${fail}`,success>0?'success':'error');
  addLog('INFO',`广播完成: ${success}/${targets.length}`);
  btn.disabled=false; btn.textContent='🚀 开始广播';
}

function renderBcHistory(){
  const el=document.getElementById('bc-history');
  if(!bcHistory.length){el.innerHTML='<div style="font-size:12px;color:var(--text-dim);">暂无记录</div>';return;}
  el.innerHTML=bcHistory.slice(0,5).map(r=>`
    <div style="border-left:3px solid var(--accent);padding:8px 12px;border-radius:0 8px 8px 0;background:var(--surface2);margin-bottom:10px;">
      <div style="font-size:12px;font-weight:600;">${r.text}</div>
      <div style="font-size:10px;color:var(--text-dim);margin-top:2px;">${r.time}</div>
      <div style="display:flex;gap:6px;margin-top:5px;">
        <span class="chip chip-green" style="font-size:9px;">✓ ${r.success}</span>
        ${r.fail?`<span class="chip chip-red" style="font-size:9px;">✗ ${r.fail}</span>`:''}
      </div>
    </div>`).join('');
  const badge=document.getElementById('bc-badge');
  badge.style.display=''; badge.textContent=bcHistory.length;
}

async function quickBroadcast(){
  const targets=document.getElementById('quick-targets').value.split(',').map(t=>t.trim()).filter(Boolean);
  const text=document.getElementById('quick-msg').value.trim();
  closeModal('broadcast-quick');
  if(!targets.length||!text){showToast('请填写完整','error');return;}
  let ok=0,fail=0;
  for(const t of targets){const res=await TG('sendMessage',{chat_id:t,text});if(res.ok)ok++;else fail++;await sleep(300);}
  showToast(`发送完成 ✓${ok} ✗${fail}`,ok>0?'success':'error');
  addLog('INFO',`快速广播: ${ok}/${targets.length} 成功`);
}

// ═══ COMMANDS ═══
async function loadCommands(){
  const container=document.getElementById('cmd-list-container');
  container.innerHTML='<div style="text-align:center;padding:24px;color:var(--text-dim);font-size:12px;"><span class="loading"></span> 加载中...</div>';
  const res=await TG('getMyCommands');
  if(!res.ok){container.innerHTML=`<div style="color:var(--accent3);padding:20px;">${res.description}</div>`;return;}
  const cmds=res.result;
  document.getElementById('cmd-badge').textContent=cmds.length;
  if(!cmds.length){container.innerHTML='<div style="text-align:center;padding:30px;color:var(--text-dim);">暂无命令，点击「+ 添加命令」</div>';return;}
  container.innerHTML=cmds.map(c=>`
    <div class="cmd-item">
      <span class="cmd-slug">/${c.command}</span>
      <span class="cmd-desc">${c.description}</span>
      <div class="action-btns">
        <button class="icon-btn danger" onclick="deleteSingleCommand('${c.command}')" title="删除">🗑</button>
      </div>
    </div>`).join('');
  addLog('INFO',`加载了 ${cmds.length} 个命令`);
}

async function addCommand(){
  const cmd=document.getElementById('new-cmd-name').value.trim().replace(/^\//,'');
  const desc=document.getElementById('new-cmd-desc').value.trim();
  const errEl=document.getElementById('add-cmd-error');
  if(!cmd||!desc){errEl.style.display='block';errEl.textContent='请填写命令名和描述';return;}
  const existing=await TG('getMyCommands');
  const cmds=existing.ok?existing.result:[];
  const updated=[...cmds.filter(c=>c.command!==cmd),{command:cmd,description:desc}];
  const res=await TG('setMyCommands',{commands:updated});
  if(res.ok){
    closeModal('add-cmd');
    document.getElementById('new-cmd-name').value='';
    document.getElementById('new-cmd-desc').value='';
    errEl.style.display='none';
    await loadCommands();
    showToast(`✅ 命令 /${cmd} 已添加`,'success');
    addLog('INFO',`添加命令: /${cmd} - ${desc}`);
  } else {
    errEl.style.display='block';errEl.textContent='❌ '+res.description;
  }
}

async function deleteSingleCommand(cmd){
  const existing=await TG('getMyCommands');
  const updated=existing.ok?existing.result.filter(c=>c.command!==cmd):[];
  const res=await TG('setMyCommands',{commands:updated});
  if(res.ok){await loadCommands();showToast(`已删除 /${cmd}`,'success');addLog('WARN',`删除命令: /${cmd}`);}
  else showToast(res.description,'error');
}

async function deleteAllCommands(){
  if(!confirm('确定要清除所有命令吗？')) return;
  const res=await TG('deleteMyCommands');
  if(res.ok){await loadCommands();showToast('已清除所有命令','success');addLog('WARN','清除所有命令');}
  else showToast(res.description,'error');
}

// ═══ SETTINGS ═══
async function loadWebhookInfo(){
  const res=await TG('getWebhookInfo');
  const el=document.getElementById('webhook-info');
  if(!res.ok){el.textContent='获取失败: '+res.description;return;}
  const w=res.result;
  el.innerHTML=w.url
    ?`<span style="color:var(--accent)">✅ 已设置 Webhook</span>\nURL: ${w.url}\n待处理: ${w.pending_update_count} 条${w.last_error_message?'\n<span style="color:var(--accent3)">最近错误: '+w.last_error_message+'</span>':''}`
    :`<span style="color:var(--accent4)">⚠️ 未设置（轮询模式）</span>\n待处理更新: ${w.pending_update_count}`;
}

async function setWebhook(){
  const url=document.getElementById('webhook-url').value.trim();
  if(!url){showToast('请输入 URL','error');return;}
  const res=await TG('setWebhook',{url});
  if(res.ok){showToast('✅ Webhook 已设置','success');addLog('INFO','设置 Webhook: '+url);loadWebhookInfo();}
  else{showToast('❌ '+res.description,'error');addLog('ERROR','Webhook 设置失败: '+res.description);}
}

async function deleteWebhook(){
  const res=await TG('deleteWebhook',{drop_pending_updates:false});
  if(res.ok){showToast('Webhook 已删除','success');addLog('WARN','删除 Webhook');loadWebhookInfo();}
  else showToast(res.description,'error');
}

async function testConnection(){
  const t0=Date.now();
  const res=await TG('getMe');
  const ping=Date.now()-t0;
  if(res.ok){showToast(`✅ 连接正常 | 延迟 ${ping}ms`,'success');addLog('INFO',`连接测试成功, 延迟 ${ping}ms`);}
  else{showToast('❌ '+res.description,'error');addLog('ERROR','连接测试失败');}
}

async function switchToken(){
  const newToken=document.getElementById('new-token-input').value.trim();
  if(!newToken){showToast('请输入新 Token','error');return;}
  const oldToken=BOT_TOKEN;
  BOT_TOKEN=newToken;
  const res=await TG('getMe');
  if(res.ok){
    botInfo=res.result;
    document.getElementById('sidebar-botname').textContent='@'+botInfo.username;
    document.getElementById('sidebar-token').textContent='token: '+newToken.substring(0,8)+'...';
    document.getElementById('current-token-display').value=newToken;
    document.getElementById('getme-raw').textContent=JSON.stringify(botInfo,null,2);
    showToast('✅ 切换 Token 成功','success');
    addLog('INFO','切换 Token → @'+botInfo.username);
    loadWebhookInfo();
  } else {
    BOT_TOKEN=oldToken;
    showToast('❌ 新 Token 无效','error');
    addLog('ERROR','切换 Token 失败: '+res.description);
  }
}

function toggleCurrentToken(){
  const i=document.getElementById('current-token-display');
  i.type=i.type==='password'?'text':'password';
}

function copyToken(){
  navigator.clipboard.writeText(BOT_TOKEN).then(()=>showToast('Token 已复制','success'));
}

// ═══ LOGS ═══
function addLog(level,msg){
  const time=new Date().toLocaleTimeString('zh-CN',{hour12:false});
  logEntries.unshift({time,level,msg});
  if(logEntries.length>300) logEntries.pop();
  if(currentPage==='logs') renderLogs();
}

function renderLogs(){
  const filter=document.getElementById('log-filter')?.value||'全部级别';
  const search=(document.getElementById('log-search')?.value||'').toLowerCase();
  const t=document.getElementById('log-terminal');
  const cls={INFO:'log-info',WARN:'log-warn',ERROR:'log-error'};
  const shown=logEntries.filter(e=>{
    if(filter!=='全部级别'&&e.level!==filter) return false;
    if(search&&!e.msg.toLowerCase().includes(search)) return false;
    return true;
  });
  t.innerHTML=shown.length
    ?shown.map(e=>`<div class="log-line"><span class="log-time">[${e.time}]</span><span class="${cls[e.level]||'log-info'}">[${e.level}]</span><span style="color:var(--text);opacity:0.85;">${e.msg}</span></div>`).join('')
    :'<div class="log-line"><span class="log-time">[--:--:--]</span><span class="log-info">[INFO]</span><span style="color:var(--text-dim)">暂无日志</span></div>';
}

function clearLogs(){logEntries=[];renderLogs();showToast('日志已清空','success');}

function exportLogs(){
  const txt=logEntries.map(e=>`[${e.time}] [${e.level}] ${e.msg}`).join('\n');
  const a=document.createElement('a');
  a.href=URL.createObjectURL(new Blob([txt],{type:'text/plain'}));
  a.download=`botpanel_${Date.now()}.txt`;
  a.click();
  showToast('日志已导出','success');
}

// ═══ UTILS ═══
let toastTimer;
function showToast(msg,type='success'){
  const t=document.getElementById('toast');
  document.getElementById('toast-msg').textContent=msg;
  document.getElementById('toast-icon').textContent=type==='success'?'✓':'✕';
  t.className=`toast ${type} show`;
  clearTimeout(toastTimer);
  toastTimer=setTimeout(()=>t.classList.remove('show'),3000);
}

function openModal(id){document.getElementById('modal-'+id).classList.add('open');}
function closeModal(id){document.getElementById('modal-'+id).classList.remove('open');}
document.querySelectorAll('.modal-overlay').forEach(m=>m.addEventListener('click',e=>{if(e.target===m)m.classList.remove('open');}));
const sleep=ms=>new Promise(r=>setTimeout(r,ms));

addLog('INFO','BotPanel 已加载，请输入 Token 连接 Bot...');
</script>
</body>
</html>
