<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1, viewport-fit=cover">
<title>Pushpender Kumar | DevOps & Cloud Engineer (Fresher)</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link href="https://fonts.googleapis.com/css2?family=Bricolage+Grotesque:wght@600;800&family=Inter+Tight:wght@400;500;600&family=JetBrains+Mono:wght@500&display=swap" rel="stylesheet">
<style>
:root{--bg:#f3f6ff;--ink:#0b1220;--mut:#4a5875;--glass:rgba(255,255,255,.7);--line:rgba(60,80,140,.18);--c1:#0891b2;--c2:#6d28d9;--c3:#ea580c;--ok:#059669;--term:#0b1220;color-scheme:light;box-sizing:border-box;padding-top:env(safe-area-inset-top,0px);padding-bottom:env(safe-area-inset-bottom,0px)}
@media (prefers-color-scheme:dark){:root:not([data-theme="light"]){--bg:#060b1a;--ink:#eaf2ff;--mut:#93a4c8;--glass:rgba(18,28,56,.62);--line:rgba(120,160,255,.2);--c1:#22d3ee;--c2:#8b5cf6;--c3:#fb923c;--ok:#34d399;color-scheme:dark}}
:root[data-theme="dark"]{--bg:#060b1a;--ink:#eaf2ff;--mut:#93a4c8;--glass:rgba(18,28,56,.62);--line:rgba(120,160,255,.2);--c1:#22d3ee;--c2:#8b5cf6;--c3:#fb923c;--ok:#34d399;color-scheme:dark}
html{scroll-behavior:smooth;scroll-padding-top:env(safe-area-inset-top,0px)}
*{box-sizing:border-box}
body{margin:0;background:var(--bg);color:var(--ink);font:400 17px/1.6 "Inter Tight",system-ui,sans-serif;overflow-x:hidden}
body:before{content:"";position:fixed;inset:0;background-image:linear-gradient(var(--line) 1px,transparent 1px),linear-gradient(90deg,var(--line) 1px,transparent 1px);background-size:56px 56px;opacity:.35;mask-image:radial-gradient(ellipse at 50% 0,#000 20%,transparent 75%);-webkit-mask-image:radial-gradient(ellipse at 50% 0,#000 20%,transparent 75%);pointer-events:none}
.aur{position:fixed;inset:0;overflow:hidden;pointer-events:none;z-index:0}
.aur i{position:absolute;width:46vw;height:46vw;border-radius:50%;filter:blur(90px);opacity:.38;animation:drift 18s ease-in-out infinite alternate}
.aur i:nth-child(1){background:var(--c1);top:-14vw;left:-10vw}
.aur i:nth-child(2){background:var(--c2);top:10vw;right:-14vw;animation-delay:-6s}
.aur i:nth-child(3){background:var(--c3);bottom:-22vw;left:28vw;opacity:.22;animation-delay:-11s}
@keyframes drift{to{transform:translate(6vw,5vw) scale(1.18)}}
#spot{position:fixed;inset:0;pointer-events:none;z-index:1;background:radial-gradient(420px circle at var(--mx,50%) var(--my,30%),rgba(120,160,255,.13),transparent 70%)}
.wrap{position:relative;z-index:2;max-width:1120px;margin:0 auto;padding:0 22px}
h1,h2,h3{font-family:"Bricolage Grotesque",Georgia,serif;margin:0;line-height:1.02}
h1{font-size:clamp(46px,8.4vw,98px);font-weight:800;letter-spacing:-.035em}
h2{font-size:clamp(30px,4.4vw,48px);font-weight:800;letter-spacing:-.025em;margin-bottom:10px}
h3{font-size:21px;font-weight:600}
.grad{background:linear-gradient(95deg,var(--c1),var(--c2) 55%,var(--c3));-webkit-background-clip:text;background-clip:text;color:transparent;background-size:200% auto;animation:shine 7s linear infinite}
@keyframes shine{to{background-position:200% center}}
section{padding:64px 0}
a{color:var(--c1)}
button{font:inherit;cursor:pointer;color:inherit}
button:focus-visible,a:focus-visible{outline:3px solid var(--c1);outline-offset:3px}
.glass{background:var(--glass);border:1px solid var(--line);border-radius:18px;backdrop-filter:blur(14px);-webkit-backdrop-filter:blur(14px);transition:border-color .25s,transform .25s,box-shadow .25s}
.glass:hover{border-color:var(--c1);box-shadow:0 10px 40px -12px var(--c1)}
.top{display:flex;justify-content:space-between;align-items:center;padding:20px 0;gap:14px}
.top nav{display:flex;gap:6px}
.top nav a{color:var(--mut);text-decoration:none;font-weight:500;padding:6px 12px;border-radius:999px}
.top nav a:hover{color:var(--ink);background:var(--glass)}
.logo{font:800 20px "Bricolage Grotesque",serif;letter-spacing:-.02em}
.ghost{background:var(--glass);border:1px solid var(--line);border-radius:999px;padding:7px 14px}
.hero{display:grid;grid-template-columns:1.1fr .9fr;gap:36px;align-items:center;padding:34px 0 40px}
.pill{display:inline-flex;gap:9px;align-items:center;padding:7px 14px;border-radius:999px;border:1px solid var(--line);background:var(--glass);font-weight:500;font-size:15px;margin-bottom:22px}
.pill b{width:9px;height:9px;border-radius:50%;background:var(--ok);box-shadow:0 0 0 0 var(--ok);animation:ping 1.8s infinite}
@keyframes ping{70%{box-shadow:0 0 0 10px transparent}100%{box-shadow:0 0 0 0 transparent}}
.type{font:600 clamp(20px,2.6vw,28px)/1.3 "Bricolage Grotesque",serif;margin:18px 0 12px;min-height:1.4em}
.type u{text-decoration:none;color:var(--c1)}
.type span{display:inline-block;width:2px;height:1em;background:var(--c1);margin-left:3px;vertical-align:-3px;animation:blink 1s steps(1) infinite}
@keyframes blink{50%{opacity:0}}
.lead{color:var(--mut);max-width:54ch;margin:0 0 26px;font-size:18px}
.cta{display:flex;flex-wrap:wrap;gap:12px}
.btn{display:inline-block;padding:13px 22px;border-radius:12px;border:1px solid var(--line);background:var(--glass);text-decoration:none;font-weight:600;color:var(--ink);transition:transform .2s}
.btn:hover{transform:translateY(-3px)}
.btn.p{background:linear-gradient(95deg,var(--c1),var(--c2));border:0;color:#fff;box-shadow:0 10px 30px -10px var(--c2)}
.term{background:var(--term);color:#d7e3ff;border-radius:18px;border:1px solid var(--line);box-shadow:0 30px 80px -30px var(--c2);overflow:hidden}
.term header{display:flex;align-items:center;gap:7px;padding:12px 16px;border-bottom:1px solid rgba(255,255,255,.1)}
.term header i{width:11px;height:11px;border-radius:50%;background:#ff5f57}.term header i:nth-child(2){background:#febc2e}.term header i:nth-child(3){background:#28c840}
.term header em{margin-left:auto;font:500 13px "JetBrains Mono",monospace;color:#8fa4d4;font-style:normal}
.term pre{margin:0;padding:16px 18px;font:500 13.5px/1.9 "JetBrains Mono",monospace;min-height:268px;white-space:pre-wrap}
.term .ok{color:#34d399}.term .cm{color:#8fa4d4}
.term .pb{height:5px;background:rgba(255,255,255,.08)}.term .pb i{display:block;height:100%;background:linear-gradient(90deg,#22d3ee,#8b5cf6,#fb923c);transition:width .5s}
.term footer{display:flex;justify-content:space-between;align-items:center;padding:10px 16px;font:500 13px "JetBrains Mono",monospace;color:#8fa4d4}
.term footer button{background:rgba(255,255,255,.08);border:0;border-radius:8px;padding:5px 12px;color:#d7e3ff}
.stats{display:grid;grid-template-columns:repeat(auto-fit,minmax(220px,1fr));gap:18px}
.stat{padding:24px}
.stat b{display:block;font:800 clamp(38px,5vw,56px)/1 "Bricolage Grotesque",serif;margin-bottom:8px}
.stat span{color:var(--mut)}
.mq{overflow:hidden;border-block:1px solid var(--line);padding:16px 0;mask-image:linear-gradient(90deg,transparent,#000 12%,#000 88%,transparent);-webkit-mask-image:linear-gradient(90deg,transparent,#000 12%,#000 88%,transparent);position:relative;z-index:2}
.mq div{display:flex;gap:44px;width:max-content;animation:run 32s linear infinite;font:700 22px "Bricolage Grotesque",serif;color:var(--mut)}
.mq div:hover{animation-play-state:paused}
@keyframes run{to{transform:translateX(-50%)}}
.tabs{display:flex;flex-wrap:wrap;gap:8px;margin:18px 0}
.tab{border:1px solid var(--line);background:var(--glass);border-radius:999px;padding:8px 18px;font-weight:500}
.tab[aria-pressed="true"]{background:linear-gradient(95deg,var(--c1),var(--c2));border-color:transparent;color:#fff}
.flow{display:flex;align-items:center;flex-wrap:wrap;gap:0;margin:26px 0}
.node{width:112px;text-align:center;padding:14px 8px;background:var(--glass);border:1px solid var(--line);border-radius:16px;transition:all .3s}
.node span{display:block;font-size:30px}
.node small{display:block;color:var(--mut);font-size:13px}
.node[aria-current="true"]{border-color:var(--c1);transform:translateY(-6px) scale(1.06);box-shadow:0 14px 40px -10px var(--c1)}
.lk{flex:1;min-width:14px;height:4px;border-radius:2px;background:var(--line);position:relative;overflow:hidden}
.lk.on:after{content:"";position:absolute;inset:0;background:linear-gradient(90deg,transparent,var(--c1),var(--c2),transparent);background-size:60% 100%;background-repeat:no-repeat;animation:fl 1.1s linear infinite}
@keyframes fl{from{background-position:-70% 0}to{background-position:170% 0}}
.detail{padding:22px 26px;border-left:4px solid var(--c1)}
.detail p{margin:8px 0 0;color:var(--mut)}
.ctl{display:flex;gap:10px;margin-top:14px;align-items:center;flex-wrap:wrap}
.chips{display:flex;flex-wrap:wrap;gap:10px}
.chip{padding:9px 15px;border-radius:12px;font-weight:600;background:var(--glass);border:1px solid var(--line);transition:all .2s}
.chip:hover{transform:translateY(-3px);border-color:var(--c2);box-shadow:0 8px 24px -10px var(--c2)}
.chip em{font-style:normal;font-weight:400;font-size:13px;color:var(--mut);margin-left:8px}
.chip.t{border-style:dashed}
.two{display:grid;grid-template-columns:repeat(auto-fit,minmax(290px,1fr));gap:20px}
.two .glass{padding:24px}
.two ul{padding-left:20px;margin:12px 0 0}.two li{margin:7px 0;color:var(--mut)}
.tl{list-style:none;padding:0;margin:26px 0 0;border-left:3px solid;border-image:linear-gradient(var(--c1),var(--c2),var(--c3)) 1}
.tl li{padding:0 0 26px 26px;position:relative}
.tl li:before{content:"";position:absolute;left:-9px;top:6px;width:15px;height:15px;border-radius:50%;background:var(--bg);border:3px solid var(--c1)}
.tl time{color:var(--c1);font-weight:600;font-size:15px}
.tl p{margin:4px 0 0;color:var(--mut)}
.note{color:var(--mut);font-size:15px;margin:4px 0 0}
.fin{text-align:center;padding:56px 24px;margin-bottom:50px}
.fin .cta{justify-content:center;margin-top:22px}
.rv{opacity:0;transform:translateY(26px);transition:opacity .7s,transform .7s}
.sp{position:fixed;top:0;left:0;height:3px;z-index:50;background:linear-gradient(90deg,var(--c1),var(--c2),var(--c3))}
.cards{display:grid;grid-template-columns:repeat(auto-fit,minmax(320px,1fr));gap:22px;margin-top:22px}
.card{padding:26px;display:flex;flex-direction:column;gap:12px;height:100%}
.card .m{font:800 34px "Bricolage Grotesque",serif}
.card p{margin:0;color:var(--mut)}
.card ul{padding-left:20px;margin:0;color:var(--mut)}
.card li{margin:6px 0}
.tags{display:flex;flex-wrap:wrap;gap:8px}
.tags span,.roles span{font-size:14px;padding:5px 12px;border-radius:999px;border:1px solid var(--line);background:var(--glass)}
.roles{display:flex;flex-wrap:wrap;gap:8px;margin:0 0 22px}
.roles span{font-weight:600;color:var(--c1)}
.rv.in{opacity:1;transform:none}
@media (max-width:860px){.hero{grid-template-columns:1fr}.top nav{display:none}.node{width:92px}}
@media (prefers-reduced-motion:reduce){*{animation:none!important;transition:none!important}.rv{opacity:1;transform:none}}
</style>
</head>
<body>
<div class="aur"><i></i><i></i><i></i></div><div id="spot"></div>
<div id="root"></div>
<script src="https://cdnjs.cloudflare.com/ajax/libs/react/18.3.1/umd/react.production.min.js"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/react-dom/18.3.1/umd/react-dom.production.min.js"></script>
<script src="https://cdn.jsdelivr.net/npm/htm@3.1.1/dist/htm.umd.js"></script>
<script>
const {useState,useEffect,useRef}=React;
const html=htm.bind(React.createElement);
const LI="https://www.linkedin.com/in/pushpender-kumar-5280b7226/",GH="https://github.com/PushpenderKumar7505";
const RM=matchMedia("(prefers-reduced-motion:reduce)").matches;

function useSeen(){const r=useRef(),[s,set]=useState(false);
  useEffect(()=>{const o=new IntersectionObserver(e=>{if(e[0].isIntersecting){set(true);o.disconnect()}},{threshold:.2});o.observe(r.current);return()=>o.disconnect()},[]);return[r,s]}
function Rv({children,className=""}){const[r,s]=useSeen();return html`<div ref=${r} className=${"rv "+className+(s?" in":"")}>${children}</div>`}
function Count({to,suffix="",pre=""}){const[r,s]=useSeen(),[v,setV]=useState(RM?to:0);
  useEffect(()=>{if(!s||RM)return;const t0=performance.now();let f;const k=n=>{const x=Math.min((n-t0)/1400,1);setV(Math.round(to*(1-Math.pow(1-x,3))));if(x<1)f=requestAnimationFrame(k)};f=requestAnimationFrame(k);return()=>cancelAnimationFrame(f)},[s]);
  return html`<b ref=${r} className="grad">${pre}${v}${suffix}</b>`}

function Typer(){const W=["CI/CD pipelines","AWS infrastructure","Ansible playbooks","Kubernetes deployments","things nobody repeats by hand"],[t,setT]=useState(RM?W[0]:"");
  useEffect(()=>{if(RM)return;let i=0,j=0,d=false,h;const k=()=>{const w=W[i];if(!d){j++;setT(w.slice(0,j));if(j===w.length){d=true;h=setTimeout(k,1500);return}}else{j--;setT(w.slice(0,j));if(j===0){d=false;i=(i+1)%W.length}}h=setTimeout(k,d?35:70)};k();return()=>clearTimeout(h)},[]);
  return html`<div className="type">I build <u>${t}</u><span></span></div>`}

const LOG=[["$ git push origin main","cm"],["✔ GitHub webhook received","ok"],["✔ Jenkins: stage 1 checkout","ok"],["✔ Jenkins: stage 2 scp playbooks → ansible-node","ok"],["✔ Jenkins: stage 3 remote execute","ok"],["✔ ansible-playbook ec2.yml → EC2 + SG + key pair","ok"],["✔ ansible-playbook pod.yml → kubernetes-node","ok"],["✔ kubectl get pods → Running","ok"],["Done in 2m 41s. Manual console: 15+ min.","cm"]];
function Term(){const[n,setN]=useState(RM?LOG.length:0),[on,setOn]=useState(!RM);
  useEffect(()=>{if(!on)return;const h=setInterval(()=>setN(x=>{if(x>=LOG.length){clearInterval(h);setOn(false);return x}return x+1}),650);return()=>clearInterval(h)},[on]);
  const sec=Math.round(n/LOG.length*161);
  return html`<div className="term"><header><i></i><i></i><i></i><em>aws-provisioning · ap-south-1</em></header>
  <pre>${LOG.slice(0,n).map((l,i)=>html`<div key=${i} className=${l[1]}>${l[0]}</div>`)}${on?"▍":""}</pre>
  <div className="pb"><i style=${{width:(n/LOG.length*100)+"%"}}></i></div>
  <footer><span>${Math.floor(sec/60)}m ${String(sec%60).padStart(2,"0")}s</span><button onClick=${()=>{setN(0);setOn(true)}}>Replay pipeline</button></footer></div>`}

const PROJ={
 "Jenkins → Ansible → Kubernetes":{repo:"Devops-automation-jenkins-ansible",steps:[
  ["GitHub","Push","A push fires a webhook. Nobody opens a console.","🐙"],
  ["Jenkins","3 stages","Checkout, SCP transfer, remote execute. The pipeline moves the playbooks to the Ansible node and starts them.","🏗️"],
  ["Ansible","Control node","ec2.yml and pod.yml run from here. Passwordless SSH to the Kubernetes server; ansible -m ping returned 0 failures.","📜"],
  ["AWS EC2","ec2.yml","The amazon.aws collection creates the EC2 instance, security group, AMI selection and key pair from code.","☁️"],
  ["Kubernetes","pod.yml","Triggered remotely over SSH. Deploys a multi-container pod on the c7i.flex.large server in ap-south-1.","☸️"],
  ["Running","kubectl","Pod status confirmed Running with kubectl. Three EC2 instances: Jenkins, Ansible, Kubernetes.","✅"]]},
 "Jenkins EC2 provisioning":{repo:"Jenkins-ansible-aws-ec2-provisioning",steps:[
  ["Code push","GitHub","A commit lands in the repository.","🐙"],
  ["Webhook","Event","GitHub calls Jenkins on every push, across 2 repositories. No polling, no manual build.","🔔"],
  ["Jenkins","Parameterized","One job, many inputs. Every run is versioned and auditable.","🏗️"],
  ["Script","Bash","Version-controlled scripts call the AWS API in place of console clicks.","📟"],
  ["IAM","Least privilege","The automation user only gets the permissions it needs to provision.","🔐"],
  ["EC2 ready","Under 3 min","Instance provisioned. 100% of manual console steps removed, 15+ minutes down to under 3.","✅"]]}
};
function Projects(){const names=Object.keys(PROJ),[n,setN]=useState(names[0]),[i,setI]=useState(0),[auto,setAuto]=useState(!RM);
  const pr=PROJ[n],s=pr.steps[i],L=pr.steps.length;
  useEffect(()=>{if(!auto)return;const h=setInterval(()=>setI(x=>(x+1)%L),2300);return()=>clearInterval(h)},[auto,n]);
  const pick=j=>{setAuto(false);setI(j)};
  return html`<div>
    <div className="tabs" role="group" aria-label="Project">${names.map(k=>html`<button key=${k} className="tab" aria-pressed=${k===n} onClick=${()=>{setN(k);setI(0)}}>${k}</button>`)}</div>
    <div className="flow">${pr.steps.map((x,j)=>html`<${React.Fragment} key=${j}>${j>0?html`<div className=${"lk"+(j<=i?" on":"")}></div>`:null}<button className="node" aria-current=${j===i} onClick=${()=>pick(j)}><span>${x[3]}</span>${x[0]}<small>${x[1]}</small></button><//>`)}</div>
    <div className="glass detail" aria-live="polite"><h3>${s[0]}: ${s[1]}</h3><p>${s[2]}</p></div>
    <div className="ctl"><button className="ghost" onClick=${()=>setAuto(!auto)}>${auto?"Pause":"Auto-play"}</button>
      <button className="ghost" onClick=${()=>pick((i+1)%L)}>Next stage</button>
      <a href=${GH+"/"+pr.repo}>Open repository: ${pr.repo}</a></div></div>`}

const SK=[["EC2","AWS","p"],["S3","AWS","p"],["IAM","AWS","p"],["VPC","AWS","p"],["Security Groups","AWS","p"],["CloudWatch","AWS","t"],["Jenkins","CI/CD","p"],["GitHub Webhooks","CI/CD","p"],["Bash","CI/CD","p"],["Ansible","Config","p"],["Terraform","Config","t"],["Docker","Containers","p"],["Kubernetes","Containers","p"],["kubectl","Containers","p"],["Linux (Ubuntu)","OS","p"],["YAML","OS","p"],["Git and GitHub","OS","p"],["Prometheus","Monitoring","t"],["Grafana","Monitoring","t"]];
function Skills(){const cats=["All",...new Set(SK.map(x=>x[1]))],[c,setC]=useState("All");
  return html`<div><div className="tabs">${cats.map(k=>html`<button key=${k} className="tab" aria-pressed=${k===c} onClick=${()=>setC(k)}>${k}</button>`)}</div>
  <div className="chips">${SK.filter(x=>c==="All"||x[1]===c).map(x=>html`<span key=${x[0]} className=${"chip"+(x[2]==="t"?" t":"")}>${x[0]}<em>${x[2]==="p"?"used in projects":"training-level"}</em></span>`)}</div></div>`}

function Progress(){const[w,setW]=useState(0);useEffect(()=>{const f=()=>{const h=document.documentElement;setW(h.scrollTop/((h.scrollHeight-h.clientHeight)||1)*100)};addEventListener("scroll",f,{passive:true});return()=>removeEventListener("scroll",f)},[]);return html`<div className="sp" style=${{width:w+"%"}}></div>`}
function Tilt({children,className=""}){const r=useRef();const mv=e=>{if(RM)return;const b=r.current.getBoundingClientRect(),x=(e.clientX-b.left)/b.width-.5,y=(e.clientY-b.top)/b.height-.5;r.current.style.transform=`perspective(800px) rotateY(${x*7}deg) rotateX(${-y*7}deg) translateY(-4px)`};return html`<div ref=${r} className=${"glass "+className} onPointerMove=${mv} onPointerLeave=${()=>{r.current.style.transform=""}}>${children}</div>`}
function Copy(){const[c,setC]=useState(false);const go=()=>{try{navigator.clipboard.writeText("pushpender7505@gmail.com").catch(()=>{})}catch(e){}setC(true);setTimeout(()=>setC(false),1800)};return html`<a className="btn" href="mailto:pushpender7505@gmail.com" onClick=${go}>${c?"Email copied":"Copy email"}</a>`}
const WORK=[{t:"Jenkins → Ansible → Kubernetes on AWS",m:"100% automated",d:"One GitHub push provisions EC2 and deploys a running Kubernetes pod. No manual steps.",b:["3-stage Jenkins pipeline: Checkout, SCP Transfer, Remote Execute","Ansible ec2.yml (amazon.aws) creates EC2, security group, AMI and key pair","Passwordless SSH: ansible -m ping returned 0 failures","3 EC2 instances in ap-south-1: Jenkins, Ansible, Kubernetes"],s:["Jenkins","Ansible","Kubernetes","AWS EC2","SSH/SCP","Ubuntu"],r:"Devops-automation-jenkins-ansible"},{t:"Automated AWS EC2 provisioning via Jenkins",m:"15 min → under 3 min",d:"A GitHub webhook triggers a parameterized Jenkins job that provisions EC2 in place of console work.",b:["Parameterized Bash scripts run through Jenkins jobs","GitHub webhooks across 2 repositories","IAM least-privilege policies for the automation user","100% of manual console clicks eliminated"],s:["Jenkins","GitHub Webhooks","AWS EC2","IAM","Bash","Ubuntu"],r:"Jenkins-ansible-aws-ec2-provisioning"}];
function App(){const[th,setTh]=useState(null);
  useEffect(()=>{const m=e=>{document.documentElement.style.setProperty("--mx",e.clientX+"px");document.documentElement.style.setProperty("--my",e.clientY+"px")};addEventListener("pointermove",m);return()=>removeEventListener("pointermove",m)},[]);
  const flip=()=>{const d=th?th==="dark":matchMedia("(prefers-color-scheme:dark)").matches;const v=d?"light":"dark";setTh(v);document.documentElement.dataset.theme=v};
  const tools=["AWS","Jenkins","Ansible","Kubernetes","Docker","Linux","Terraform","Git","Bash","Prometheus","Grafana","IAM"];
  return html`<div>
  <div className="wrap">
    <${Progress}/><div className="top"><span className="logo grad">PK</span>
      <nav><a href="#work">Projects</a><a href="#proof">Pipelines</a><a href="#skills">Skills</a><a href="#where">Honest status</a><a href="#path">Experience</a><a href="#edu">Education</a><a href="#contact">Contact</a></nav>
      <button className="ghost" onClick=${flip} aria-label="Switch light or dark theme">Theme</button></div>
    <header className="hero">
      <div><div className="pill"><b></b>Open to work · Immediate joiner · Delhi NCR and remote</div>
        <h1>Pushpender <span className="grad">Kumar</span></h1>
        <${Typer}/>
        <p className="lead"><b>DevOps and Cloud Engineer, fresher.</b> I turn 15-minute manual AWS provisioning into a git push. Jenkins, Ansible and Kubernetes on EC2, built and documented end to end.</p>
        <div className="roles"><span>DevOps Engineer</span><span>Cloud Engineer</span><span>Cloud Support Engineer</span><span>Cloud Infrastructure Engineer</span></div><div className="cta"><a className="btn p" href=${GH}>View my GitHub</a><a className="btn" href=${LI}>LinkedIn</a><${Copy}/></div></div>
      <${Term}/>
    </header>
  </div>
  <div className="mq" aria-hidden="true"><div>${[...tools,...tools].map((t,i)=>html`<span key=${i}>${t}</span>`)}</div></div>
  <div className="wrap">
    <section><${Rv}><div className="stats">
      <div className="glass stat"><${Count} to=${80} suffix="%"/><span>less time to provision an EC2 instance: 15+ min down to under 3</span></div>
      <div className="glass stat"><${Count} to=${100} suffix="%"/><span>of manual console steps removed across 2 CI/CD projects</span></div>
      <div className="glass stat"><${Count} to=${0}/><span>failures on ansible -m ping across the 3-node setup</span></div>
    </div><p className="note">Results come from my lab and training projects, documented in the linked repositories.</p><//></section>
    <section id="work"><${Rv}><h2>Projects that <span className="grad">actually ship</span></h2><p className="note">Both are public repositories with the full pipeline documented.</p>
      <div className="cards">${WORK.map(w=>html`<${Tilt} key=${w.t} className="card"><div className="m grad">${w.m}</div><h3>${w.t}</h3><p>${w.d}</p><ul>${w.b.map(x=>html`<li key=${x}>${x}</li>`)}</ul><div className="tags">${w.s.map(x=>html`<span key=${x}>${x}</span>`)}</div><a href=${GH+"/"+w.r}>Open repository: ${w.r}</a><//>`)}</div><//></section>
    <section id="proof"><${Rv}><h2>Two pipelines, <span className="grad">stage by stage</span></h2><p className="note">Watch it run, or click any stage.</p><${Projects}/><//></section>
    <section id="skills"><${Rv}><h2>Skills, with <span className="grad">proof level</span></h2><p className="note">Solid outline means used in a project. Dashed means covered in training, not yet shipped.</p><${Skills}/><//></section>
    <section id="where"><${Rv}><h2>Where I <span className="grad">honestly</span> stand</h2>
      <div className="two"><div className="glass"><h3>What is solid</h3><ul><li>Jenkins pipelines triggered by GitHub webhooks.</li><li>Ansible playbooks that create AWS resources and deploy to Kubernetes.</li><li>Linux servers, SSH key authentication, IAM least privilege.</li></ul></div>
      <div className="glass"><h3>What is not there yet</h3><ul><li>My results come from lab and training projects, not production systems.</li><li>Terraform is training-level. A hands-on project is in progress.</li><li>Croma Campus gave me training certificates, not an AWS exam certification.</li></ul></div></div><//></section>
    <section id="path"><${Rv}><h2>Experience and <span className="grad">training</span></h2>
      <ol className="tl">
        <li><time>Jul 2024 to Oct 2024</time><h3>Backend Developer Intern, Mentobile Technology</h3><p>CodeIgniter (MVC), MySQL schemas and CRUD, Git branching and code reviews.</p></li>
        <li><time>Jan 2025 to Jun 2025</time><h3>Market Research Associate, Precise Research Solution</h3><p>Cleaned and analysed datasets, wrote decision-support reports for stakeholders.</p></li>
        <li><time>Sep 2025 to Mar 2026</time><h3>AWS and DevOps Infrastructure Training, Croma Campus</h3><p>NASSCOM-certified, Wipro Credential Partner. Linux, Git, Jenkins, Docker, Kubernetes, AWS, Terraform, Ansible, Prometheus, Grafana.</p></li>
        <li><time>Jul 2026</time><h3>Associate, Incident Response (FTH), UnitedLex</h3><p>Data breach investigations and PII/PHI classification using Relativity and Microsoft 365.</p></li>
      </ol><//></section>
    <section id="edu"><${Rv}><h2>Education, <span className="grad">training</span> and what is next</h2>
      <div className="cards">
        <${Tilt} className="card"><h3>B.Tech, Computer Science and Engineering</h3><p>GLA University, Mathura. 2020 to 2024.</p><//>
        <${Tilt} className="card"><h3>AWS and DevOps Infrastructure Training</h3><p>Croma Campus, NASSCOM-certified, Wipro Credential Partner. Sep 2025 to Mar 2026.</p><p>Linux administration, Git and GitHub workflows, Jenkins, Docker, Kubernetes, AWS (EC2, S3, IAM, VPC, CloudWatch), Terraform, Ansible, Prometheus, Grafana.</p><//>
        <${Tilt} className="card"><h3>Other courses</h3><ul><li>Web Development Bootcamp, JOVAC</li><li>Front-End Development (HTML and CSS), Great Learning</li><li>Course on Computer Concepts (CCC), NIELIT</li></ul><//>
        <${Tilt} className="card"><h3>Currently building</h3><ul><li>Terraform infrastructure as code on AWS</li><li>Advanced Kubernetes</li></ul><//>
      </div><//></section>
    <${Rv}><div className="glass fin" id="contact"><h2>Need someone who <span className="grad">automates</span> the boring parts?</h2><p className="note">Send me the role. I will tell you plainly where I fit and where I do not.</p>
      <div className="cta"><a className="btn p" href="mailto:pushpender7505@gmail.com">pushpender7505@gmail.com</a><a className="btn" href=${LI}>LinkedIn</a><a className="btn" href=${GH}>GitHub</a></div></div><//>
  </div></div>`}
ReactDOM.createRoot(document.getElementById("root")).render(html`<${App}/>`);
</script>
</body>
</html>
