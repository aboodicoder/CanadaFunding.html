
<!doctype html>
<html lang="en">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width,initial-scale=1" />
  }
  html,body{height:100%;margin:0;font-family:Inter, "Segoe UI", Roboto, sans-serif;background:linear-gradient(180deg,#07070a,#0f0f13);color:#fff}
  .wrap{max-width:980px;margin:28px auto;padding:18px}
  .banner{
    display:flex;gap:12px;padding:12px 16px;border-radius:8px;background:linear-gradient(90deg, rgba(255,59,59,0.12), rgba(255,30,30,0.05));
    border:2px solid rgba(255,59,59,0.12);align-items:center;
  }
  .banner strong{font-size:16px;color:#fff}
  .banner small{color:var(--muted);opacity:0.95}
  .panel{margin-top:18px;background:linear-gradient(180deg, rgba(255,255,255,0.02), rgba(255,255,255,0.01));padding:18px;border-radius:10px;border:1px solid rgba(255,255,255,0.02)}
  .title{font-size:20px;color:var(--red);margin:0 0 6px}
  .subtitle{color:var(--muted);margin:0 0 12px}
  table{width:100%;border-collapse:collapse;margin-top:10px}
  th,td{padding:10px;border-bottom:1px dashed rgba(255,255,255,0.03);text-align:left;font-size:14px}
  th{color:var(--muted);font-weight:600}
  .total{font-weight:900;color:#ffdede;font-size:20px}
  .sysbox{margin-top:12px;padding:12px;border-radius:8px;background:#0a0a0a;border:1px solid rgba(255,255,255,0.03);font-size:13px;color:var(--muted);white-space:pre-wrap}
  .readmore{margin-top:14px;display:flex;justify-content:space-between;align-items:center}
  .rm-btn{background:transparent;border:2px solid rgba(255,255,255,0.04);padding:8px 12px;border-radius:8px;color:var(--muted);cursor:pointer}
  .reveal{display:none;margin-top:14px;padding:12px;border-radius:8px;background:linear-gradient(180deg,#08331a,#032813);color:#cfead9;border:1px solid rgba(0,0,0,0.3)}
  .muted{color:var(--muted)}
  .disclaimer{margin-top:14px;padding:10px;border-radius:8px;background:linear-gradient(90deg, rgba(255,255,255,0.02), rgba(255,255,255,0.01));color:var(--muted);font-size:13px}
  .cta{margin-top:12px;display:flex;gap:8px}
  .btn-primary{background:var(--red);border:none;color:#fff;padding:10px 14px;border-radius:8px;cursor:pointer}
  .btn-ghost{background:transparent;border:1px solid rgba(255,255,255,0.04);color:var(--muted);padding:10px 12px;border-radius:8px;cursor:pointer}
  /* accessible focus */
  button:focus{outline:3px solid rgba(255,255,255,0.06);outline-offset:2px}
  @media (max-width:720px){
    .wrap{padding:12px}
  }
</style>
</head>
<body>
  <div class="wrap">
    <div class="banner" role="status" aria-live="polite">
      <div>
        <div><small>This page is intentionally a threat for overdue payments.</small></div>
      </div>
      <div style="margin-left:auto;text-align:right">
        <div style="font-weight:700;color:#fff">Demo Invoice</div>
        <div class="muted" style="font-size:12px">For entertainment only</div>
      </div>
    </div>

    <div class="panel" role="main" aria-labelledby="head">
      <h2 id="head" class="title">Outstanding Account Summary (DEMO)</h2>
      <p class="subtitle">This is a Canadian Agency message warning you to pay up overdue payments/invoices.</p>

      <table aria-hidden="false">
        <thead>
          <tr><th>Item</th><th>Details</th><th style="text-align:right">Amount (CAD)</th></tr>
        </thead>
        <tbody id="itemsBody">
          <!-- JS will populate items -->
        </tbody>
        <tfoot>
          <tr><td colspan="2" style="text-align:right" class="muted">Total Due</td><td style="text-align:right" class="total" id="totalAmount">$0</td></tr>
        </tfoot>
      </table>

      <div class="sysbox" id="sysbox" aria-live="polite">
        <!-- decorative system info inserted by JS -->
      </div>

      <div class="readmore">
        <button class="rm-btn" id="readMoreBtn">Read more</button>
        <div class="muted" style="font-size:13px">Click "Read more" for important information.</div>
      </div>

      <div id="reveal" class="reveal" role="status" aria-live="polite">
        <strong>This is a harmless prank — you owe nothing.</strong>
        <p style="margin:8px 0 0">No accounts were accessed. The invoice and “system details” are decorative only and collected from the browser for display (user agent, screen size). Do not use deceptive notices to threaten or coerce people.</p>
      </div>

      <div class="disclaimer">
        <strong>Reminder:</strong> This demo is safe and intended for playful use with consent. If you want a more subtle demonstration, include a visible disclaimer or obtain explicit consent from the viewer.
      </div>

      <div style="margin-top:12px" class="cta">
        <button class="btn-primary" id="regenBtn">Regenerate Fake Invoice</button>
        <button class="btn-ghost" id="downloadBtn">Download (JSON)</button>
      </div>
    </div>
  </div>

<script>
  // Fake invoice generator (harmless)
  const ITEMS_POOL = [
    {item:'Outstanding Hosting Fees', price: 1299},
    {item:'Premium Support (unpaid)', price: 4999},
    {item:'License Renewal (enterprise)', price: 24999},
    {item:'Security Audit (past due)', price: 7999},
    {item:'Cloud Credits (overuse)', price: 18999},
    {item:'Data Migration Service', price: 9999},
    {item:'Custom Integration', price: 15999},
    {item:'Late Payment Penalty', price: 1299},
    {item:'Administrative Fee', price: 199},
    {item:'Processor Charge', price: 349},
    {item:'Device Management Fee', price: 499},
    {item:'Service Suspension Fee', price: 1299}
  ];

  function pickRandom(arr, n){
    const copy = arr.slice();
    const res = [];
    for (let i=0;i<n && copy.length;i++){
      const idx = Math.floor(Math.random()*copy.length);
      res.push(copy.splice(idx,1)[0]);
    }
    return res;
  }

  function formatUSD(n){ return '$' + n.toLocaleString(); }

  function buildInvoice(){
    const count = 4 + Math.floor(Math.random()*6); // 4..9 items
    const items = pickRandom(ITEMS_POOL, count).map(it=>{
      const mult = 1 + Math.floor(Math.random()*10);
      const qty = (Math.random() < 0.35) ? (1 + Math.floor(Math.random()*5)) : 1;
      const amount = it.price * qty * mult;
      return {desc: it.item + (qty>1 ? ` ×${qty}` : ''), amount};
    });
    const total = items.reduce((s,i)=>s+i.amount,0);
    return {items, total, generatedAt: new Date().toISOString()};
  }

  function getSystemDecorativeInfo(){
    // Only use non-sensitive, browser-available info; label clearly
    return {
      'Browser userAgent': navigator.userAgent,
      'Platform': navigator.platform,
      'Screen size': `${screen.width}×${screen.height}`,
      'Language': navigator.language || navigator.userLanguage,
      'Time (local)': new Date().toString()
    };
  }

  function render(){
    const invoice = buildInvoice();
    const tbody = document.getElementById('itemsBody');
    tbody.innerHTML = '';
    invoice.items.forEach(it=>{
      const tr = document.createElement('tr');
      tr.innerHTML = `<td>${escapeHtml(it.desc)}</td><td class="muted">Invoice #${Math.floor(Math.random()*900000+100000)}</td><td style="text-align:right">${formatUSD(it.amount)}</td>`;
      tbody.appendChild(tr);
    });
    document.getElementById('totalAmount').textContent = formatUSD(invoice.total);

    // system info box: decorative only
    const sys = getSystemDecorativeInfo();
    const sysbox = document.getElementById('sysbox');
    let out = 'Decorative system details (for demo only):\n\n';
    for (const k in sys) out += `${k}: ${sys[k]}\n`;
    sysbox.textContent = out;

    // attach the latest generated invoice data to element for download
    document.getElementById('downloadBtn').dataset.invoice = JSON.stringify(invoice, null, 2);
  }

  // sanitize text for HTML (small helper)
  function escapeHtml(s){
    return String(s).replace(/[&<>"']/g, ch => ({'&':'&amp;','<':'&lt;','>':'&gt;','"':'&quot;',"'":'&#39;'}[ch]));
  }

  document.getElementById('regenBtn').addEventListener('click', ()=> render());
  document.getElementById('readMoreBtn').addEventListener('click', ()=>{
    document.getElementById('reveal').style.display = 'block';
    document.getElementById('readMoreBtn').style.display = 'none';
  });
  document.getElementById('downloadBtn').addEventListener('click', ()=>{
    const data = document.getElementById('downloadBtn').dataset.invoice || '{}';
    const blob = new Blob([data], {type:'application/json'});
    const url = URL.createObjectURL(blob);
    const a = document.createElement('a');
    a.href = url;
    a.download = 'fake-invoice.json';
    document.body.appendChild(a);
    a.click();
    a.remove();
    URL.revokeObjectURL(url);
  });

  // initial render
  render();
</script>
</body>
</html>
