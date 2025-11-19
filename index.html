<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="utf-8"/>
<meta http-equiv="Cache-Control" content="no-cache, no-store, must-revalidate"/>
<meta http-equiv="Pragma" content="no-cache"/>
<meta http-equiv="Expires" content="0"/>
<meta name="viewport" content="width=device-width, initial-scale=1, maximum-scale=5, user-scalable=yes"/>
<title>Health & Wellness Dashboard</title>
<link href="https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:wght@400;600;700&display=swap" rel="stylesheet"/>
<script src="https://cdn.plot.ly/plotly-2.32.0.min.js"></script>
<script src="https://cdn.jsdelivr.net/npm/papaparse@5.4.1/papaparse.min.js"></script>
<style>
:root {
  --bg:#f8fafc; --text:#0f172a; --muted:#64748b; --card:#ffffff; --border:#e2e8f0;
  --bg-secondary:#f1f5f9;
  --us:#2563eb; --can:#9333ea; --accent:#10b981; --warn:#f59e0b; --error:#ef4444;
  --shadow:0 1px 3px rgba(15,23,42,.08),0 4px 12px rgba(15,23,42,.05);
  --shadow-lg:0 4px 6px rgba(15,23,42,.07),0 12px 24px rgba(15,23,42,.08);
}
body.dark {
  --bg:#0a0e1a; --text:#f1f5f9; --muted:#94a3b8; --card:#0f1629; --border:#1e293b;
  --bg-secondary:#141b2e;
  --shadow:0 1px 3px rgba(0,0,0,.3),0 8px 20px rgba(0,0,0,.25);
  --shadow-lg:0 4px 6px rgba(0,0,0,.4),0 12px 28px rgba(0,0,0,.35);
}
*{box-sizing:border-box;transition:background-color .25s ease,color .25s ease,border-color .25s ease;}
html,body{height:100%;margin:0;padding:0;overflow-x:hidden;}
body{padding:24px;font-family:'Plus Jakarta Sans',Inter,system-ui,-apple-system,sans-serif;background:var(--bg);color:var(--text);line-height:1.6;}
.header{display:flex;align-items:center;justify-content:space-between;margin-bottom:8px;flex-wrap:wrap;gap:12px;}
h1{font-size:32px;margin:0;font-weight:700;letter-spacing:-.02em;background:linear-gradient(135deg,var(--us),var(--can));-webkit-background-clip:text;-webkit-text-fill-color:transparent;background-clip:text;}
.status-bar{display:flex;align-items:center;gap:16px;font-size:13px;color:var(--muted);margin-bottom:20px;flex-wrap:wrap;}
.status-item{display:flex;align-items:center;gap:6px;padding:6px 12px;background:var(--bg-secondary);border-radius:8px;border:1px solid var(--border);}
.status-indicator{width:8px;height:8px;border-radius:50%;background:var(--muted);animation:pulse 2s ease-in-out infinite;}
.status-indicator.success{background:var(--accent);}
.status-indicator.error{background:var(--error);}
@keyframes pulse{0%,100%{opacity:1;}50%{opacity:.5;}}
.tabs{display:flex;gap:8px;margin:20px 0;padding-bottom:4px;border-bottom:2px solid var(--border);overflow-x:auto;-webkit-overflow-scrolling:touch;}
.tab-button{padding:10px 18px;border:none;border-radius:10px 10px 0 0;background:transparent;cursor:pointer;color:var(--muted);font-weight:600;font-size:14px;white-space:nowrap;position:relative;transition:all .2s ease;}
.tab-button:hover{color:var(--text);background:var(--bg-secondary);}
.tab-button.active{color:var(--us);background:var(--card);box-shadow:0 -2px 0 var(--us) inset;}
.tab-button:focus{outline:2px solid var(--us);outline-offset:2px;}
.tab-content{display:none;animation:fadeIn .3s ease;}
.tab-content.active{display:block;}
@keyframes fadeIn{from{opacity:0;transform:translateY(10px);}to{opacity:1;transform:translateY(0);}}
.section{margin-bottom:32px;}
.section-header{display:flex;align-items:center;justify-content:space-between;margin-bottom:16px;}
.section-title{font-size:18px;font-weight:700;color:var(--text);margin:0;}
.grid-4{display:grid;grid-template-columns:repeat(4,1fr);gap:16px;}
.grid-3{display:grid;grid-template-columns:repeat(3,1fr);gap:18px;}
.grid-2{display:grid;grid-template-columns:repeat(2,1fr);gap:18px;}
.card{background:var(--card);border:1px solid var(--border);border-radius:16px;padding:20px;box-shadow:var(--shadow);transition:box-shadow .3s ease;}
.card:hover{box-shadow:var(--shadow-lg);}
.legend{font-size:13px;color:var(--muted);font-weight:600;text-transform:uppercase;letter-spacing:.05em;margin-bottom:12px;}
.kpi{background:linear-gradient(135deg,var(--card),var(--bg-secondary));border:1px solid var(--border);border-radius:14px;padding:18px;box-shadow:var(--shadow);transition:transform .2s ease,box-shadow .2s ease;}
.kpi:hover{transform:translateY(-2px);box-shadow:var(--shadow-lg);}
.kpi h3{margin:0 0 8px 0;font-size:11px;color:var(--muted);text-transform:uppercase;letter-spacing:.08em;font-weight:700;}
.kpi .val{font-size:28px;font-weight:700;color:var(--text);line-height:1;}
.toolbar{display:flex;gap:12px;align-items:center;flex-wrap:wrap;margin-bottom:20px;padding:16px;background:var(--bg-secondary);border-radius:12px;border:1px solid var(--border);}
.pill{display:inline-flex;align-items:center;gap:8px;font-size:13px;font-weight:600;color:var(--text);}
select{appearance:none;background:var(--card);color:var(--text);border:1px solid var(--border);border-radius:10px;padding:9px 32px 9px 12px;min-width:180px;font-size:14px;font-weight:600;cursor:pointer;box-shadow:var(--shadow);background-image:url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='12' height='12' viewBox='0 0 12 12'%3E%3Cpath fill='%2364748b' d='M6 8L2 4h8z'/%3E%3C/svg%3E");background-repeat:no-repeat;background-position:right 10px center;}
select:hover{border-color:var(--us);}
select:focus{outline:2px solid var(--us);outline-offset:2px;border-color:var(--us);}
.theme-toggle{padding:8px 16px;font-size:13px;font-weight:600;border-radius:10px;border:1px solid var(--border);background:var(--card);cursor:pointer;color:var(--text);box-shadow:var(--shadow);transition:all .2s ease;}
.theme-toggle:hover{transform:translateY(-1px);box-shadow:var(--shadow-lg);border-color:var(--us);}
.theme-toggle:focus{outline:2px solid var(--us);outline-offset:2px;}
.partners-list{list-style:none;margin:0;padding:0;}
.partners-list li{display:grid;grid-template-columns:auto 1fr auto;align-items:center;gap:12px;padding:16px;margin-bottom:10px;background:var(--bg-secondary);border:1px solid var(--border);border-radius:12px;transition:all .2s ease;min-width:0;cursor:pointer;}
.partners-list li:hover{border-color:var(--us);box-shadow:var(--shadow);}
.partners-list .name{font-weight:700;color:var(--text);font-size:15px;word-wrap:break-word;overflow-wrap:break-word;min-width:0;}
.partners-list .meta{font-size:12px;color:var(--muted);display:flex;align-items:center;gap:8px;flex-wrap:wrap;justify-content:flex-end;}
.partners-list .meta a{padding:4px 8px;border-radius:6px;background:rgba(16,185,129,.1);}
.badge{display:inline-block;padding:3px 8px;border-radius:6px;font-size:11px;font-weight:700;text-transform:uppercase;letter-spacing:.03em;}
.badge.us{background:rgba(37,99,235,.15);color:var(--us);}
.badge.can{background:rgba(147,51,234,.15);color:var(--can);}
.badge.payment{background:rgba(16,185,129,.15);color:var(--accent);}
.badge.payment-employee-paid{background:rgba(37,99,235,.15);color:#2563eb;}
.badge.payment-employee-reimb{background:rgba(245,158,11,.15);color:#f59e0b;}
.badge.payment-company-paid{background:rgba(16,185,129,.15);color:#10b981;}
table{width:100%;border-collapse:collapse;}
thead tr{border-bottom:2px solid var(--border);}
th{text-align:left;padding:12px;font-weight:700;text-transform:uppercase;font-size:11px;letter-spacing:.08em;color:var(--muted);}
td{padding:14px 12px;border-bottom:1px solid var(--border);}
tbody tr:hover{background:var(--bg-secondary);}
.empty-state{text-align:center;padding:48px 24px;color:var(--muted);}
.empty-state-icon{font-size:48px;margin-bottom:16px;opacity:.5;}
@media(max-width:1200px){.grid-4{grid-template-columns:repeat(2,1fr);}.grid-3{grid-template-columns:repeat(2,1fr);}}
@media(max-width:768px){
body{padding:16px;}
h1{font-size:24px;}
.grid-4,.grid-3,.grid-2{grid-template-columns:1fr;}
.kpi .val{font-size:24px;}
.header{flex-direction:column;align-items:flex-start;}
.tabs{margin:16px -16px;padding:0 16px 4px;border-bottom:1px solid var(--border);}
.tab-button{padding:8px 14px;font-size:13px;}
.toolbar{flex-direction:column;align-items:stretch;}
select{width:100%;}
.partners-list li{grid-template-columns:1fr;gap:8px;padding:12px;}
.partners-list .name{font-size:14px;}
.partners-list .meta{justify-content:flex-start;margin-top:4px;}
.section-title{font-size:16px;}
.status-bar{flex-direction:column;align-items:flex-start;gap:8px;}
table{font-size:13px;}
th,td{padding:10px 8px;}
}
@media(max-width:480px){
.kpi{padding:14px;}
.card{padding:16px;}
h1{font-size:20px;}
.kpi h3{font-size:10px;}
.kpi .val{font-size:20px;}
.badge{font-size:10px;padding:2px 6px;}
.partners-list .name{font-size:13px;}
.partners-list .meta{font-size:11px;}
.tab-button{padding:6px 10px;font-size:12px;}
}
</style>
</head>
<body>
<div class="header">
<h1>Health & Wellness Dashboard</h1>
<button id="themeToggle" class="theme-toggle" aria-label="Toggle theme">🌙 Dark Mode</button>
</div>
<div class="status-bar">
<div class="status-item"><span class="status-indicator" id="statusIndicator"></span><span id="loadStatus">Initializing...</span></div>
<div class="status-item" id="lastUpdated" style="display:none;"><span>📅</span><span id="lastUpdatedText">—</span></div>
</div>
<div class="tabs" role="tablist">
<button class="tab-button active" role="tab" aria-selected="true" onclick="openTab('current')">Overview</button>
<button class="tab-button" role="tab" aria-selected="false" onclick="openTab('clubInsights')">Club Insights</button>
<button class="tab-button" role="tab" aria-selected="false" onclick="openTab('employerPaid')">Employer-Sponsored</button>
<button class="tab-button" role="tab" aria-selected="false" onclick="openTab('active')">Active Partners</button>
<button class="tab-button" role="tab" aria-selected="false" onclick="openTab('changelog')">Changelog</button>
</div>
<div class="tab-content active" id="current" role="tabpanel">
<div class="section">
<div class="grid-4 kpis">
<div class="kpi"><h3>Total Members</h3><div class="val" id="kpiTotal">—</div></div>
<div class="kpi"><h3>Black Card</h3><div class="val" id="kpiBC">—</div></div>
<div class="kpi"><h3>10NR Members</h3><div class="val" id="kpi10NR">—</div></div>
<div class="kpi"><h3>Promo Codes</h3><div class="val" id="kpiPromo">—</div></div>
</div>
</div>
<div class="section">
<h3 class="section-title">Regional Distribution</h3>
<div class="grid-3">
<div class="card"><div class="legend">Total Members by Region</div><div id="regionTotalChart"></div></div>
<div class="card"><div class="legend">Black Card by Region</div><div id="regionBCChart"></div></div>
<div class="card"><div class="legend">10NR by Region</div><div id="region10NRChart"></div></div>
</div>
</div>
<div class="section">
<h3 class="section-title">Monthly Trends</h3>
<div class="grid-2">
<div class="card"><div class="legend">United States Signups</div><div id="impactUS"></div></div>
<div class="card"><div class="legend">Canada Signups</div><div id="impactCAN"></div></div>
</div>
</div>
<div class="section">
<div class="card"><div class="legend">Top 5 Promotion Codes (US vs Canada)</div><div id="promoChart"></div></div>
</div>
</div>
<div class="tab-content" id="clubInsights" role="tabpanel">
<div class="card">
<div class="toolbar">
<label class="pill">Club <select id="clubSelect" aria-label="Select club"><option value="__ALL__" selected>All Clubs</option></select></label>
<label class="pill">Month <select id="monthSelect" aria-label="Select month"><option value="all" selected>All Months</option></select></label>
</div>
<div class="grid-4 kpis">
<div class="kpi"><h3>Total Members</h3><div class="val" id="ckpiTotal">—</div></div>
<div class="kpi"><h3>Black Card</h3><div class="val" id="ckpiBC">—</div></div>
<div class="kpi"><h3>10NR Members</h3><div class="val" id="ckpi10NR">—</div></div>
<div class="kpi"><h3>Promo Codes</h3><div class="val" id="ckpiCodes">—</div></div>
</div>
<div class="grid-2" style="margin-top:24px;">
<div class="card"><div class="legend">Regional Split</div><div id="clubRegionDonut"></div></div>
<div class="card"><div class="legend">Top Promotion Codes</div><div id="clubUsage"></div></div>
</div>
<div class="card" style="margin-top:24px;"><div class="legend">Monthly Signup Trend</div><div id="clubTrend"></div></div>
</div>
<div class="card" style="margin-top:24px;"><div class="legend">Top 5 Clubs by Usage (US vs Canada)</div><div id="topClubsChart"></div></div>
</div>
<div class="tab-content" id="employerPaid" role="tabpanel">
<div class="card">
<h3 class="section-title" style="margin-bottom:20px;">Employer-Sponsored Programs</h3>
<table><thead><tr><th>Company Name</th><th style="text-align:right;">Total Members</th></tr></thead>
<tbody><tr><td><strong>Pansophia</strong></td><td id="kpiPansophia" style="text-align:right;font-weight:700;">—</td></tr>
<tr><td><strong>ASAMA Coldwater Manufacturing</strong></td><td id="kpiAsama" style="text-align:right;font-weight:700;">—</td></tr></tbody></table>
</div>
</div>
<div class="tab-content" id="active" role="tabpanel">
<div class="card">
<div class="section-header">
<h3 class="section-title">Active Partnership Network</h3>
<div id="activeStatus" class="status-item"><span class="status-indicator"></span><span>Loading...</span></div>
</div>
<div class="grid-2" style="margin-bottom:24px;">
<div class="card"><div class="legend">Geographic Distribution</div><div id="partnersByRegion"></div></div>
<div class="card"><div class="legend">Payment Arrangement Types</div><div id="paymentByRegion"></div></div>
</div>
<div><div class="legend" style="margin-bottom:16px;">Partner Directory</div><ul id="partnersList" class="partners-list" style="max-height:600px;overflow-y:auto;"></ul></div>
</div>
</div>
<div class="tab-content" id="changelog" role="tabpanel">
<div class="card">
<h2 class="section-title" style="margin-bottom:20px;">Recent Updates</h2>
<ul style="line-height:2;color:var(--muted);">
<li><strong>Active Partners:</strong> Added payment arrangement information and regional payment breakdown</li>
<li><strong>Active Partners:</strong> Added partner list with regional breakdown (East / West / Canada)</li>
<li><strong>UI Improvements:</strong> Enhanced visuals and responsive design</li>
<li><strong>Performance:</strong> Optimized chart rendering and data loading</li>
</ul>
</div>
</div>
<script>
const CFG={
  CODES:["CLEMENSBC","CLEMENSWC","MTPCORPWC","CORPBC","CORP15","CORPFMBC","CORPFM15","CORP10","PFCORP10","PFCORPBC"],
  CSV:"https://docs.google.com/spreadsheets/d/e/2PACX-1vQ8iruNQ-H8vQvlNMSNXiUtOoxI1b8lEyL7YMBOifM2os3qyRTdmQ2_1V2oKk4vMlQifynBfxrN-u-F/pub?output=csv",
  PARTNERS:"https://docs.google.com/spreadsheets/d/e/2PACX-1vTXJ4Wm19clU5g5BOxIi_nLA10BAbLuI-s7eYpk9yRmLWCcmcb7ekDGlXldv9buG0GYgJxSLpiRWRXa/pub?output=csv",
  EMPLOYER:[
    {company:"Pansophia",groupKey:"Pansophia",url:"https://docs.google.com/spreadsheets/d/e/2PACX-1vSTKsFVL_lAR2kSk8EHhMlc8-q_Xy1eVJ5kYFXk1ZuQo6Ukpp-GnFNRR6o_DI7rVBXxGvhmCGeecgi1/pub?gid=1580598102&single=true&output=csv",target:"kpiPansophia"},
    {company:"ASAMA Coldwater Manufacturing",groupKey:"ASAMABC",url:"https://docs.google.com/spreadsheets/d/e/2PACX-1vSTKsFVL_lAR2kSk8EHhMlc8-q_Xy1eVJ5kYFXk1ZuQo6Ukpp-GnFNRR6o_DI7rVBXxGvhmCGeecgi1/pub?gid=1118993687&single=true&output=csv",target:"kpiAsama"}
  ]
};
const ST={data:[],filtered:[],months:[],loaded:false,partnersLoaded:false};
function hasCode(n){return CFG.CODES.some(c=>(n||"").toUpperCase().includes(c));}
function normReg(v){const s=(v||"").toUpperCase().trim();if(["CA","CAN","CANADA"].includes(s))return"CAN";if(["US","USA","UNITED STATES"].includes(s))return"US";return s;}
function monthKey(d){return d.getFullYear()+"-"+String(d.getMonth()+1).padStart(2,"0");}
function monthLbl(k){const[y,m]=k.split("-");return new Date(y,m-1).toLocaleString("default",{month:"short",year:"numeric"});}
function setStatus(msg,type){
  const s=document.getElementById("loadStatus"),i=document.getElementById("statusIndicator");
  s.textContent=msg;i.className="status-indicator";
  if(type==="success"){i.classList.add("success");s.style.color="var(--accent)";}
  else if(type==="error"){i.classList.add("error");s.style.color="var(--error)";}
}
function pal(){
  const d=document.body.classList.contains("dark");
  return{paper:d?"#0a0e1a":"#f8fafc",plot:d?"#0f1629":"#ffffff",grid:d?"#1e293b":"#e2e8f0",font:d?"#f1f5f9":"#0f172a",us:"#2563eb",can:"#9333ea",accent:"#10b981"};
}
function lay(y,x){
  const p=pal();
  return{margin:{t:20,b:50,l:60,r:20},paper_bgcolor:p.paper,plot_bgcolor:p.plot,font:{color:p.font,family:"'Plus Jakarta Sans',sans-serif",size:12},xaxis:{title:x,gridcolor:p.grid,zerolinecolor:p.grid,automargin:true},yaxis:{title:y,gridcolor:p.grid,zerolinecolor:p.grid,automargin:true},legend:{orientation:"h",y:1.12,x:0,bgcolor:"rgba(0,0,0,0)"},hovermode:"closest",autosize:true};
}
const pcfg={displayModeBar:false,responsive:true,autosizable:true};
async function loadData(){
  try{
    setStatus("Loading data...","info");
    Papa.parse(CFG.CSV,{download:true,header:true,skipEmptyLines:true,complete:result=>{
      try{
        const data=result.data||[];
        // Clean and process the data
        const processed=data.map(row=>{
          const o={};
          for(const k in row){
            o[k.trim().toLowerCase()]=row[k];
          }
          const ds=(o["created date"]||"").trim();
          o.dateParsed=new Date(ds.includes("/")?ds.replace(/(\d{1,2})\/(\d{1,2})\/(\d{4})/,"$3-$1-$2"):ds);
          return o;
        });
        ST.data=processed;
        ST.filtered=processed.filter(r=>hasCode(r["promotion name"]));
        ST.months=[...new Set(ST.filtered.map(r=>{const d=r.dateParsed;return isNaN(d)?null:monthKey(d);}).filter(Boolean))].sort();
        ST.loaded=true;
        renderCurrent(ST.filtered);
        setupClub(ST.filtered);
        renderTopClubs();
        const latest=new Date(Math.max(...ST.filtered.map(r=>r.dateParsed).filter(d=>!isNaN(d))));
        const ls=latest.toLocaleDateString("en-US",{year:"numeric",month:"short",day:"numeric"});
        document.getElementById("lastUpdated").style.display="flex";
        document.getElementById("lastUpdatedText").textContent=`Data through: ${ls}`;
        setStatus(`${ST.filtered.length} records loaded`,"success");
      }catch(e){
        console.error(e);
        setStatus("Failed to process data","error");
      }
    },error:e=>{
      console.error(e);
      setStatus("Failed to load data","error");
    }});
  }catch(e){console.error(e);setStatus("Failed to load data","error");}
}
function renderCurrent(data){
  const p=pal();
  document.getElementById("kpiTotal").textContent=data.length.toLocaleString();
  document.getElementById("kpiBC").textContent=data.filter(r=>(r["membership type"]||"").toUpperCase().includes("BLACK")).length.toLocaleString();
  document.getElementById("kpi10NR").textContent=data.filter(r=>(r["membership type"]||"").toUpperCase().includes("10NR")).length.toLocaleString();
  document.getElementById("kpiPromo").textContent=new Set(data.map(r=>(r["promotion name"]||"").trim()).filter(Boolean)).size;
  const tot={US:0,CAN:0},bc={US:0,CAN:0},nr={US:0,CAN:0};
  data.forEach(r=>{const reg=normReg(r["region"]);if(!(reg in tot))return;tot[reg]++;const m=(r["membership type"]||"").toUpperCase();if(m.includes("BLACK"))bc[reg]++;if(m.includes("10NR"))nr[reg]++;});
  Plotly.newPlot("regionTotalChart",[{x:Object.keys(tot),y:Object.values(tot),type:"bar",marker:{color:[p.us,p.can]},text:Object.values(tot),textposition:"auto",textfont:{color:"white",size:14,weight:"bold"},hovertemplate:"%{x}: %{y}<extra></extra>"}],{...lay("Members","Region"),height:300},pcfg);
  Plotly.newPlot("regionBCChart",[{x:Object.keys(bc),y:Object.values(bc),type:"bar",marker:{color:[p.us,p.can]},text:Object.values(bc),textposition:"auto",textfont:{color:"white",size:14,weight:"bold"},hovertemplate:"%{x}: %{y}<extra></extra>"}],{...lay("Members","Region"),height:300},pcfg);
  Plotly.newPlot("region10NRChart",[{x:Object.keys(nr),y:Object.values(nr),type:"bar",marker:{color:[p.us,p.can]},text:Object.values(nr),textposition:"auto",textfont:{color:"white",size:14,weight:"bold"},hovertemplate:"%{x}: %{y}<extra></extra>"}],{...lay("Members","Region"),height:300},pcfg);
  const mUS={},mCAN={};
  data.forEach(r=>{const d=r.dateParsed;if(isNaN(d))return;const k=monthKey(d);const reg=normReg(r["region"]);if(reg==="US")mUS[k]=(mUS[k]||0)+1;if(reg==="CAN")mCAN[k]=(mCAN[k]||0)+1;});
  const kUS=Object.keys(mUS).sort(),kCAN=Object.keys(mCAN).sort();
  Plotly.newPlot("impactUS",[{x:kUS.map(monthLbl),y:kUS.map(k=>mUS[k]),type:"bar",marker:{color:p.us},hovertemplate:"%{x}<br>%{y} signups<extra></extra>"}],{...lay("Signups","Month"),xaxis:{...lay().xaxis,type:"category"},height:300},pcfg);
  Plotly.newPlot("impactCAN",[{x:kCAN.map(monthLbl),y:kCAN.map(k=>mCAN[k]),type:"bar",marker:{color:p.can},hovertemplate:"%{x}<br>%{y} signups<extra></extra>"}],{...lay("Signups","Month"),xaxis:{...lay().xaxis,type:"category"},height:300},pcfg);
  const pReg={US:{},CAN:{}};
  data.forEach(r=>{const pn=(r["promotion name"]||"").trim();if(!pn)return;const reg=normReg(r["region"]);if(!(reg in pReg))return;pReg[reg][pn]=(pReg[reg][pn]||0)+1;});
  const all=new Set([...Object.keys(pReg.US),...Object.keys(pReg.CAN)]);
  const pTot={};all.forEach(pn=>pTot[pn]=(pReg.US[pn]||0)+(pReg.CAN[pn]||0));
  const top=Object.entries(pTot).sort((a,b)=>b[1]-a[1]).slice(0,5).map(([pn])=>pn);
  if(!top.length)document.getElementById("promoChart").innerHTML='<div class="empty-state"><div class="empty-state-icon">📊</div><p>No promotion data</p></div>';
  else Plotly.newPlot("promoChart",[{name:"US",x:top.map(pn=>pReg.US[pn]||0),y:top,type:"bar",orientation:"h",marker:{color:p.us}},{name:"CAN",x:top.map(pn=>pReg.CAN[pn]||0),y:top,type:"bar",orientation:"h",marker:{color:p.can}}],{...lay("","Usage"),margin:{t:20,l:180,b:50,r:20},barmode:"group",height:350},pcfg);
}
function setupClub(data){
  const cs=document.getElementById("clubSelect"),ms=document.getElementById("monthSelect");
  [...new Set(data.map(r=>(r["club name"]||"").trim()).filter(Boolean))].sort().forEach(c=>{const o=document.createElement("option");o.value=c;o.textContent=c;cs.appendChild(o);});
  ST.months.forEach(m=>{const o=document.createElement("option");o.value=m;o.textContent=monthLbl(m);ms.appendChild(o);});
  cs.onchange=ms.onchange=renderClub;
  renderClub();
}
function renderClub(){
  const p=pal();
  const c=document.getElementById("clubSelect").value;
  const m=document.getElementById("monthSelect").value;
  let rows=[...ST.filtered];
  if(c!=="__ALL__")rows=rows.filter(r=>(r["club name"]||"").trim()===c);
  if(m!=="all")rows=rows.filter(r=>{const d=r.dateParsed;return!isNaN(d)&&monthKey(d)===m;});
  document.getElementById("ckpiTotal").textContent=rows.length.toLocaleString();
  document.getElementById("ckpiBC").textContent=rows.filter(r=>(r["membership type"]||"").toUpperCase().includes("BLACK")).length.toLocaleString();
  document.getElementById("ckpi10NR").textContent=rows.filter(r=>(r["membership type"]||"").toUpperCase().includes("10NR")).length.toLocaleString();
  document.getElementById("ckpiCodes").textContent=new Set(rows.map(r=>(r["promotion name"]||"").trim()).filter(Boolean)).size;
  const rCnt={US:0,CAN:0};
  rows.forEach(r=>{const reg=normReg(r["region"]);if(rCnt[reg]!=null)rCnt[reg]++;});
  Plotly.newPlot("clubRegionDonut",[{labels:["US","CAN"],values:[rCnt.US,rCnt.CAN],type:"pie",hole:.6,marker:{colors:[p.us,p.can]},textinfo:"label+percent",hovertemplate:"%{label}: %{value}<extra></extra>"}],{paper_bgcolor:p.paper,plot_bgcolor:p.plot,font:{color:p.font,family:"'Plus Jakarta Sans',sans-serif"},showlegend:false,margin:{t:10,b:10,l:10,r:10}},pcfg);
  const pCnt={};
  rows.forEach(r=>{const pn=(r["promotion name"]||"").trim();if(pn)pCnt[pn]=(pCnt[pn]||0)+1;});
  const topCodes=Object.entries(pCnt).sort((a,b)=>b[1]-a[1]).slice(0,5);
  Plotly.newPlot("clubUsage",[{x:topCodes.map(([,cnt])=>cnt),y:topCodes.map(([pn])=>pn),type:"bar",orientation:"h",marker:{color:p.accent}}],{...lay("","Usage"),margin:{t:10,l:160,b:50,r:20},height:280},pcfg);
  const mData={};
  rows.forEach(r=>{const d=r.dateParsed;if(isNaN(d))return;const k=monthKey(d);mData[k]=(mData[k]||0)+1;});
  const mKeys=Object.keys(mData).sort();
  Plotly.newPlot("clubTrend",[{x:mKeys.map(monthLbl),y:mKeys.map(k=>mData[k]),type:"scatter",mode:"lines+markers",line:{width:3,color:p.us},marker:{size:8},hovertemplate:"%{x}<br>%{y} signups<extra></extra>"}],{...lay("Signups","Month"),xaxis:{...lay().xaxis,type:"category"},height:300},pcfg);
}
function renderTopClubs(){
  const p=pal();
  const rows=ST.filtered;
  const cUS={},cCAN={};
  rows.forEach(r=>{
    const club=(r["club name"]||"").trim();
    const promo=(r["promotion name"]||"").trim();
    const reg=normReg(r["region"]);
    if(!club||!promo)return;
    if(reg==="US"){cUS[club]=cUS[club]||{count:0,promo};cUS[club].count++;}
    if(reg==="CAN"){cCAN[club]=cCAN[club]||{count:0,promo};cCAN[club].count++;}
  });
  const all=new Set([...Object.keys(cUS),...Object.keys(cCAN)]);
  const tots={};
  all.forEach(c=>tots[c]=(cUS[c]?.count||0)+(cCAN[c]?.count||0));
  const top=Object.entries(tots).sort((a,b)=>b[1]-a[1]).slice(0,5).map(([c])=>c);
  const names=top.map(c=>{const promo=cUS[c]?.promo||cCAN[c]?.promo||"";return promo?`${c} (${promo})`:c;});
  Plotly.newPlot("topClubsChart",[{name:"US",x:top.map(c=>cUS[c]?.count||0),y:names,type:"bar",orientation:"h",marker:{color:p.us}},{name:"CAN",x:top.map(c=>cCAN[c]?.count||0),y:names,type:"bar",orientation:"h",marker:{color:p.can}}],{...lay("","Usage"),margin:{t:20,l:320,b:50,r:20},barmode:"group",height:350},pcfg);
}
function norm(s){return(s||"").toString().trim().toLowerCase();}
function findGrp(hdrs){const n=hdrs.map(h=>norm(h));const i=n.findIndex(h=>h==="group"||h==="groups"||h.includes("group"));return i>=0?hdrs[i]:hdrs[0];}
async function countGrp(url,match){
  return new Promise((res,rej)=>{
    Papa.parse(url,{download:true,header:true,skipEmptyLines:true,complete:r=>{
      try{
        const rows=r.data||[];
        if(!rows.length)return res(0);
        const hdrs=Object.keys(rows[0]);
        const key=findGrp(hdrs);
        const tot=rows.filter(row=>((row[key]||"")+"").toLowerCase().includes(match.toLowerCase())).length;
        res(tot);
      }catch(e){rej(e);}
    },error:e=>rej(e)});
  });
}
async function renderEmployer(){
  for(const emp of CFG.EMPLOYER){
    const el=document.getElementById(emp.target);
    if(!el)continue;
    el.textContent="...";
    try{
      const tot=await countGrp(emp.url,emp.groupKey);
      el.textContent=tot.toLocaleString();
    }catch(e){console.error(`Employer error for ${emp.company}:`,e);el.textContent="—";}
  }
}
function renderPartners(){
  if(ST.partnersLoaded)return;
  const statusEl=document.getElementById("activeStatus").querySelector("span:last-child");
  const listEl=document.getElementById("partnersList");
  statusEl.textContent="Loading...";
  Papa.parse(CFG.PARTNERS,{download:true,header:true,skipEmptyLines:true,complete:r=>{
    const rows=r.data||[];
    if(!rows.length){statusEl.textContent="No partners found";return;}
    const clean=rows.map(row=>{const o={};for(const k in row)o[k.trim().toLowerCase()]=(row[k]||"").trim();return o;});
    const partners=clean.map(r=>{
      const name=r["company name"]||r["company"]||"Unknown";
      let region=r["region"]||"Unknown";
      region=region.replace(/east canada|eastern canada/i,"East").replace(/west canada|western canada/i,"West").replace(/canada/i,"Canada");
      const promo=r["promotion type"]||r["promotion"]||"";
      
      // Try all possible column names for payment arrangement
      const payment=r["payment arrangement"]||r["payment arrangements"]||r["payment"]||r["payment type"]||
                    r["paymentarrangement"]||r["paymentarrangements"]||r["paymenttype"]||
                    r["employee reimbursement"]||r["company paid"]||r["employee paid"]||"";
      
      // Get supporting documents link
      const docsLink=r["supporting documents (urls)"]||r["supporting documents"]||r["supporting document"]||r["documents"]||r["document link"]||r["link"]||"";
      
      return{name,region,promo,payment,docsLink};
    });
    if(!partners.length){statusEl.textContent="No partners found";return;}
    partners.sort((a,b)=>a.name.localeCompare(b.name));
    
    // Color coordination helper function
    const getPaymentBadgeClass=(payment)=>{
      const p=payment.toLowerCase();
      if(p.includes('employee paid'))return'badge payment-employee-paid';
      if(p.includes('employee reimbursement'))return'badge payment-employee-reimb';
      if(p.includes('company paid'))return'badge payment-company-paid';
      return'badge payment';
    };
    
    listEl.innerHTML=partners.map(p=>`<li><span class="badge ${p.region==="Canada"?"can":"us"}">${p.region}</span><span class="name">${p.name}</span><span class="meta">${p.payment?`<span class="${getPaymentBadgeClass(p.payment)}">${p.payment}</span>`:""}${p.docsLink?`<a href="${p.docsLink}" target="_blank" rel="noopener noreferrer" style="color:var(--accent);text-decoration:none;font-weight:600;white-space:nowrap;display:inline-flex;align-items:center;gap:4px;">📄 Flyer</a>`:""}</span></li>`).join("");
    const rCnts=partners.reduce((acc,p)=>{acc[p.region]=(acc[p.region]||0)+1;return acc;},{});
    const regs=Object.entries(rCnts).sort((a,b)=>b[1]-a[1]);
    const p=pal();
    Plotly.newPlot("partnersByRegion",[{x:regs.map(([reg])=>reg),y:regs.map(([,cnt])=>cnt),type:"bar",marker:{color:regs.map(([reg])=>reg==="Canada"?p.can:reg==="East"?p.us:p.accent)},text:regs.map(([,cnt])=>cnt),textposition:"auto",textfont:{color:"white",size:14,weight:"bold"},hovertemplate:"%{x}: %{y}<extra></extra>"}],{...lay("Partners","Region"),height:300,margin:{t:10,l:50,r:10,b:50}},pcfg);
    
    // New chart: Payment Arrangement Types (simple bar chart)
    const paymentCounts={};
    partners.forEach(partner=>{
      if(partner.payment){
        paymentCounts[partner.payment]=(paymentCounts[partner.payment]||0)+1;
      }
    });
    
    const paymentEntries=Object.entries(paymentCounts).sort((a,b)=>b[1]-a[1]);
    
    if(paymentEntries.length>0){
      // Assign specific colors for each payment type
      const getPaymentColor=(type)=>{
        const t=type.toLowerCase();
        if(t.includes('employee paid'))return'#2563eb'; // Blue for Employee Paid
        if(t.includes('employee reimbursement'))return'#f59e0b'; // Orange for Employee Reimbursement
        if(t.includes('company paid'))return'#10b981'; // Green for Company Paid
        return p.accent; // Default color for others
      };
      
      const colors=paymentEntries.map(([type])=>getPaymentColor(type));
      
      Plotly.newPlot("paymentByRegion",[{
        x:paymentEntries.map(([type])=>type),
        y:paymentEntries.map(([,cnt])=>cnt),
        type:"bar",
        marker:{color:colors},
        text:paymentEntries.map(([,cnt])=>cnt),
        textposition:"outside",
        textfont:{color:p.font,size:14,weight:"bold"},
        hovertemplate:"%{x}: %{y} partners<extra></extra>",
        cliponaxis:false
      }],{...lay("Partners","Payment Type"),height:320,margin:{t:40,l:50,r:10,b:100},yaxis:{...lay().yaxis,rangemode:"tozero"}},pcfg);
    }else{
      document.getElementById("paymentByRegion").innerHTML='<div class="empty-state"><div class="empty-state-icon">💳</div><p>No payment arrangement data</p></div>';
    }
    
    statusEl.textContent=`${partners.length} partners`;
    ST.partnersLoaded=true;
    requestAnimationFrame(resizeCharts);
  },error:e=>{console.error("Partners error:",e);statusEl.textContent="Failed to load";}});
}
function openTab(tab){
  document.querySelectorAll(".tab-content").forEach(t=>t.classList.remove("active"));
  document.querySelectorAll(".tab-button").forEach(b=>{b.classList.remove("active");b.setAttribute("aria-selected","false");});
  const tEl=document.getElementById(tab);
  if(tEl)tEl.classList.add("active");
  const bEl=document.querySelector(`button[onclick="openTab('${tab}')"]`);
  if(bEl){bEl.classList.add("active");bEl.setAttribute("aria-selected","true");}
  if(tab==="employerPaid")renderEmployer();
  else if(tab==="active")renderPartners();
  else if(["current","clubInsights"].includes(tab)&&ST.loaded)rerender();
  requestAnimationFrame(resizeCharts);
}
function toggleTheme(){
  document.body.classList.toggle("dark");
  const isDark=document.body.classList.contains("dark");
  localStorage.setItem("theme",isDark?"dark":"light");
  document.getElementById("themeToggle").textContent=isDark?"☀️ Light Mode":"🌙 Dark Mode";
  updateChartThemes();
  requestAnimationFrame(resizeCharts);
}

function updateChartThemes(){
  const p = pal();
  const ids = [
    "regionTotalChart","regionBCChart","region10NRChart","impactUS","impactCAN","promoChart",
    "clubRegionDonut","clubUsage","clubTrend","topClubsChart","partnersByRegion","paymentByRegion"
  ];
  ids.forEach(id => {
    const el = document.getElementById(id);
    if (el && el.data) {
      Plotly.relayout(el, {
        paper_bgcolor: p.paper,
        plot_bgcolor: p.plot,
        font: { color: p.font, family: "'Plus Jakarta Sans',sans-serif", size: 12 },
        xaxis: { gridcolor: p.grid, zerolinecolor: p.grid },
        yaxis: { gridcolor: p.grid, zerolinecolor: p.grid }
      });
    }
  });
}
function resizeCharts(){
  const ids=["regionTotalChart","regionBCChart","region10NRChart","impactUS","impactCAN","promoChart","clubRegionDonut","clubUsage","clubTrend","topClubsChart","partnersByRegion","paymentByRegion"];
  ids.forEach(id=>{
    const el=document.getElementById(id);
    if(el&&el.data){
      try{
        Plotly.Plots.resize(el);
      }catch(e){
        console.warn(`Failed to resize chart ${id}:`,e);
      }
    }
  });
}
function rerender(){
  if(!ST.loaded)return;
  // Only clear and re-render charts for the active tab
  const activeTab = document.querySelector('.tab-content.active');
  if (!activeTab) return;

  // Overview tab
  if (activeTab.id === "current") {
    ["regionTotalChart","regionBCChart","region10NRChart","impactUS","impactCAN","promoChart"].forEach(id=>{
      const el=document.getElementById(id);
      if(el) el.innerHTML = "";
    });
    renderCurrent(ST.filtered);
  }
  // Club Insights tab
  else if (activeTab.id === "clubInsights") {
    ["clubRegionDonut","clubUsage","clubTrend","topClubsChart"].forEach(id=>{
      const el=document.getElementById(id);
      if(el) el.innerHTML = "";
    });
    renderClub();
    renderTopClubs();
  }
  // Active Partners tab
  else if (activeTab.id === "active") {
    ["partnersByRegion","paymentByRegion"].forEach(id=>{
      const el=document.getElementById(id);
      if(el) el.innerHTML = "";
    });
    ST.partnersLoaded = false; // Force reload for theme
    renderPartners();
  }
  setTimeout(resizeCharts,100);
}
function init(){
  if(localStorage.getItem("theme")==="dark"){document.body.classList.add("dark");document.getElementById("themeToggle").textContent="☀️ Light Mode";}
  loadData();
  document.getElementById("themeToggle").onclick=toggleTheme;
  
  // Better resize handling
  let resizeTimer;
  window.addEventListener("resize",()=>{
    clearTimeout(resizeTimer);
    resizeTimer=setTimeout(()=>{
      resizeCharts();
    },100);
  });
  
  // Also resize on window load to ensure proper initial sizing
  window.addEventListener("load",resizeCharts);
}
document.addEventListener("DOMContentLoaded",init);
</script>
</body>
</html>
