# reserve-ja-
<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1, viewport-fit=cover">
<title>Estúdio Sirlene Mendes – Reservas</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link href="https://fonts.googleapis.com/css2?family=Great+Vibes&family=Playfair+Display:ital,wght@0,600;1,500&family=Quicksand:wght@500;600;700&display=swap" rel="stylesheet">
<style>
:root{
  --bg:#ffe9f1; --bg2:#fff7fa; --card:#ffffff; --ink:#4a3a3d; --mute:#8e7a7c;
  --rose:#f8c8da; --rose2:#fde3ec; --gold:#c9a45c; --green:#5fb883;
  --line:#f8d9e5;
  box-sizing:border-box;padding-top:env(safe-area-inset-top,0px);padding-bottom:env(safe-area-inset-bottom,0px)}
@media (prefers-color-scheme:dark){:root:not([data-theme="light"]){--bg:#2d2124;--bg2:#35282b;--card:#3d2e31;--ink:#fbeceb;--mute:#d8bcba;--line:#5a4347;--rose:#6a4a4f;--rose2:#4a3438}}
:root[data-theme="dark"]{--bg:#2d2124;--bg2:#35282b;--card:#3d2e31;--ink:#fbeceb;--mute:#d8bcba;--line:#5a4347;--rose:#6a4a4f;--rose2:#4a3438}
html{scroll-padding-top:env(safe-area-inset-top,0px)}
*{box-sizing:border-box}
body{margin:0;background:linear-gradient(180deg,var(--bg2),var(--bg));background-color:var(--bg);color:var(--ink);font-family:"Quicksand","Segoe UI",system-ui,sans-serif;font-weight:500;min-height:100vh}
body::before{content:"";position:fixed;inset:0 0 auto;height:env(safe-area-inset-top,0px);background:var(--bg2);z-index:4}
.wrap{max-width:480px;margin:0 auto;padding:0 16px 48px}
header{text-align:center;padding:28px 0 4px}
.logo{width:104px;height:104px;margin:0 auto 10px;border-radius:50%;background:var(--card);display:grid;place-items:center;border:2px solid var(--gold);box-shadow:0 8px 22px rgba(201,164,92,.25);overflow:hidden}
.logo img{width:100%;height:100%;object-fit:cover}
.logo span{font-family:"Great Vibes",cursive;font-size:46px;color:var(--gold);line-height:1;padding-top:6px}
h1{font-family:"Great Vibes",cursive;font-weight:400;font-size:42px;margin:0;line-height:1.1;color:var(--ink)}
.tag{font-size:12px;letter-spacing:.28em;text-transform:uppercase;color:var(--gold);margin:4px 0 0;font-weight:700}
.divider{display:flex;align-items:center;gap:10px;justify-content:center;color:var(--gold);margin:12px auto 0;max-width:240px}
.divider::before,.divider::after{content:"";flex:1;height:1px;background:linear-gradient(90deg,transparent,var(--gold),transparent)}

.welcome{margin:20px 0 6px;background:var(--card);border-radius:26px;padding:22px 20px 18px;position:relative;border:1.5px dashed var(--rose);box-shadow:0 8px 22px rgba(248,200,218,.35)}
.welcome::before{content:"♡";position:absolute;top:-15px;left:50%;transform:translateX(-50%);background:var(--rose);color:#fff;width:30px;height:30px;border-radius:50%;display:grid;place-items:center;font-size:15px}
.welcome h3{font-family:"Playfair Display",Georgia,serif;font-style:italic;font-weight:500;font-size:20px;margin:4px 0 8px;text-align:center}
.welcome p{margin:0;font-size:15px;line-height:1.55;text-align:center;color:var(--mute)}
.welcome .sig{font-family:"Great Vibes",cursive;font-size:28px;color:var(--gold);margin-top:6px;line-height:1.1;text-align:center}

nav{position:sticky;top:env(safe-area-inset-top,0px);z-index:5;display:flex;gap:6px;background:var(--card);padding:6px;border-radius:999px;margin:20px 0 16px;box-shadow:0 6px 16px rgba(248,200,218,.5);border:1.5px solid var(--line)}
nav button{flex:1;border:0;background:transparent;color:var(--mute);font:700 13px "Quicksand",system-ui,sans-serif;padding:10px 4px;border-radius:999px;cursor:pointer;display:flex;flex-direction:column;align-items:center;gap:2px}
nav button svg{width:18px;height:18px;stroke:currentColor;fill:none;stroke-width:1.8;stroke-linecap:round;stroke-linejoin:round}
nav button[aria-selected=true]{background:var(--rose2);color:var(--ink);box-shadow:inset 0 0 0 1.5px var(--rose)}

.panel{display:none;animation:in .35s ease}
.panel.on{display:block}
@keyframes in{from{opacity:0;transform:translateY(8px)}to{opacity:1;transform:none}}
.card{background:var(--card);border-radius:26px;padding:20px;margin-bottom:14px;border:1.5px solid var(--line);box-shadow:0 8px 22px rgba(248,200,218,.3)}
h2{font-family:"Playfair Display",Georgia,serif;font-style:italic;font-weight:500;font-size:22px;margin:0 0 4px}
.step{display:flex;align-items:center;gap:10px;margin:20px 0 10px;font-weight:700;font-size:15px}
.step.first{margin-top:10px}
.step i{font-style:normal;width:26px;height:26px;border-radius:50%;background:var(--rose2);color:var(--ink);display:grid;place-items:center;font-size:13px;flex:none;border:1.5px solid var(--rose)}
.opt{display:flex;align-items:center;gap:12px;padding:12px 14px;border:1.5px solid var(--line);border-radius:16px;margin-bottom:8px;cursor:pointer}
.opt input{accent-color:var(--gold);width:20px;height:20px;flex:none}
.opt:has(input:checked){border-color:var(--rose);background:var(--rose2)}
textarea,select{width:100%;border:1.5px solid var(--line);border-radius:16px;padding:12px;font:inherit;background:var(--card);color:var(--ink)}
textarea:focus,select:focus{outline:2px solid var(--rose)}
.slots{display:grid;grid-template-columns:repeat(4,1fr);gap:8px}
.slot{border:1.5px solid var(--line);background:var(--card);color:var(--ink);border-radius:14px;padding:10px 0;font:700 14px "Quicksand",system-ui,sans-serif;cursor:pointer}
.slot:hover{border-color:var(--rose)}
.slot.on{background:var(--green);border-color:var(--green);color:#fff;transform:scale(1.04)}

.preview{margin-top:18px;border-radius:18px;background:var(--bg2);border:1.5px solid var(--line);padding:14px}
.preview b{font-size:13px;color:var(--gold);letter-spacing:.06em;text-transform:uppercase}
.preview pre{margin:8px 0 0;white-space:pre-wrap;font:500 14px/1.5 "Quicksand",system-ui,sans-serif;color:var(--ink)}
.preview.empty pre{color:var(--mute);font-style:italic}
.btn{display:block;width:100%;text-align:center;text-decoration:none;border:0;border-radius:999px;padding:15px;font:700 16px "Quicksand",system-ui,sans-serif;cursor:pointer;margin-top:14px}
.wa{background:var(--green);color:#fff;box-shadow:0 8px 18px rgba(95,184,131,.35)}
.wa[aria-disabled=true]{opacity:.4;pointer-events:none}
.pix{background:var(--rose);color:#4a3a3d;box-shadow:0 8px 18px rgba(248,200,218,.6)}
.small{font-size:13px;color:var(--mute);text-align:center;margin:10px 0 0}
p{line-height:1.55;margin:8px 0}
.note{background:var(--rose2);border:1.5px dashed var(--rose);color:var(--ink);border-radius:16px;padding:14px;font-size:14px;margin-top:14px;text-align:center}
.pay{display:flex;gap:8px;flex-wrap:wrap;margin-top:10px}
.pay span{border:1.5px solid var(--rose);background:var(--rose2);border-radius:999px;padding:6px 14px;font-size:14px;font-weight:700}
.big{font-family:"Great Vibes",cursive;font-size:38px;color:var(--gold);text-align:center;line-height:1;margin:6px 0}
.addr{display:flex;gap:12px;align-items:flex-start}
.addr svg{width:26px;height:26px;flex:none;stroke:var(--gold);fill:none;stroke-width:1.8}
footer{text-align:center;color:var(--mute);font-size:13px;margin-top:22px}
footer b{font-family:"Great Vibes",cursive;font-weight:400;font-size:24px;color:var(--gold)}
</style>
</head>
<body>
<div class="wrap">
<header>
  <div class="logo" id="logo"><span>SM</span></div>
  <h1>Estúdio Sirlene Mendes</h1>
  <p class="tag">Studio de Beleza</p>
  <div class="divider">✦</div>
</header>

<div class="welcome">
  <h3>Seja muito bem-vinda!</h3>
  <p>Aqui o seu momento é feito com carinho, cuidado e atenção a cada detalhe. Escolha o seu horário com calma, e eu confirmo tudo com você pelo WhatsApp. Será um prazer te receber!</p>
  <div class="sig">Sirlene Mendes</div>
</div>

<nav role="tablist">
  <button role="tab" aria-selected="true" data-t="reserva"><svg viewBox="0 0 24 24"><rect x="3.5" y="5" width="17" height="15" rx="3"/><path d="M8 3v4M16 3v4M3.5 10h17"/></svg>Reservar</button>
  <button role="tab" aria-selected="false" data-t="local"><svg viewBox="0 0 24 24"><path d="M12 21s7-6.2 7-11.2A7 7 0 0 0 5 9.8C5 14.8 12 21 12 21z"/><circle cx="12" cy="10" r="2.5"/></svg>Localização</button>
  <button role="tab" aria-selected="false" data-t="pagar"><svg viewBox="0 0 24 24"><rect x="3" y="6" width="18" height="13" rx="3"/><path d="M3 10.5h18M7 15h3"/></svg>Como pagar</button>
</nav>

<div class="panel on" id="reserva">
  <div class="card">
    <h2>Faça sua reserva</h2>
    <p class="small" style="text-align:left;margin-top:0">São só três passinhos ♡</p>

    <div class="step first"><i>1</i>Qual procedimento você quer?</div>
    <label class="opt"><input type="checkbox" value="Escova"> Escova</label>
    <label class="opt"><input type="checkbox" value="Progressiva"> Progressiva</label>
    <label class="opt"><input type="checkbox" value="Hidratação"> Hidratação</label>
    <label class="opt"><input type="checkbox" value="Corte"> Corte</label>
    <textarea id="extra" rows="2" placeholder="Quer acrescentar mais algum procedimento ou deixar um recadinho?"></textarea>

    <div class="step"><i>2</i>Escolha o dia</div>
    <select id="dia"></select>

    <div class="step"><i>3</i>Escolha o horário <span style="font-weight:500;color:var(--mute);font-size:13px">(7h às 19h)</span></div>
    <div class="slots" id="slots"></div>

    <div class="preview empty" id="prev">
      <b>Mensagem para a Sirlene</b>
      <pre id="msgtxt">Escolha o procedimento, o dia e o horário e a sua mensagem aparece aqui, prontinha para enviar.</pre>
    </div>
    <a class="btn wa" id="wa" aria-disabled="true" href="#" target="_blank" rel="noopener">Enviar para a Sirlene no WhatsApp</a>
    <p class="small">Seu pedido vai direto para a Sirlene, que confirma a data com você.</p>
  </div>
</div>

<div class="panel" id="local">
  <div class="card">
    <h2>Onde nos encontrar</h2>
    <div class="addr" style="margin-top:12px">
      <svg viewBox="0 0 24 24"><path d="M12 21s7-6.2 7-11.2A7 7 0 0 0 5 9.8C5 14.8 12 21 12 21z"/><circle cx="12" cy="10" r="2.5"/></svg>
      <div>Rua João Soares da Silva,<br>Travessa Flamengo, nº 16<br>Jardim Silvina · São Bernardo do Campo – SP</div>
    </div>
    <div class="note">Atendemos de segunda a sábado, das 7h às 19h. Domingo fechado.</div>
  </div>
</div>

<div class="panel" id="pagar">
  <div class="card">
    <h2>Como pagar</h2>
    <div class="big">sinal de 50%</div>
    <p style="text-align:center">Para garantir o seu horário, pedimos um sinal de 50% do valor do procedimento.</p>
    <p style="margin-bottom:0"><b>Formas de pagamento</b></p>
    <div class="pay"><span>Pix</span><span>Dinheiro</span><span>Cartão</span></div>
    <a class="btn pix" href="https://link.mercadopago.com.br/studiosirlenemendes" target="_blank" rel="noopener">Pagar o sinal via Pix</a>
    <div class="note">O sinal não é devolvido em caso de cancelamento ou falta.</div>
  </div>
</div>

<footer><b>Sirlene Mendes</b><br>Obrigada pela preferência ♡</footer>
</div>

<script>
var WA="https://wa.me/5511949075554";
var sel=null,dias=["domingo","segunda","terça","quarta","quinta","sexta","sábado"];
var dsel=document.getElementById("dia"),box=document.getElementById("slots");
function p(n){return String(n).padStart(2,"0")}
var tabs=document.querySelectorAll("nav button");
tabs.forEach(function(b){b.onclick=function(){
  tabs.forEach(function(x){x.setAttribute("aria-selected",x===b)});
  document.querySelectorAll(".panel").forEach(function(s){s.classList.toggle("on",s.id===b.dataset.t)});
  window.scrollTo({top:0,behavior:"smooth"});
}});
var d=new Date(2026,10,16),fim=new Date(2026,11,31);
while(d<=fim){
  if(d.getDay()!==0){
    var o=document.createElement("option");
    o.value=p(d.getDate())+"/"+p(d.getMonth()+1)+"/2026";
    o.textContent=dias[d.getDay()]+", "+o.value;
    dsel.appendChild(o);
  }
  d=new Date(d.getFullYear(),d.getMonth(),d.getDate()+1);
}
for(var m=7*60;m<=19*60;m+=30){
  var t=p(Math.floor(m/60))+"h"+p(m%60);
  var b=document.createElement("button");
  b.type="button";b.className="slot";b.textContent=t;
  b.onclick=function(){sel=this.textContent;[].forEach.call(box.children,function(x){x.classList.remove("on")});this.classList.add("on");upd()};
  box.appendChild(b);
}
var EMPTY="Escolha o procedimento, o dia e o horário e a sua mensagem aparece aqui, prontinha para enviar.";
function upd(){
  var l=[].map.call(document.querySelectorAll("input[type=checkbox]:checked"),function(c){return c.value});
  var e=document.getElementById("extra").value.trim();
  var wa=document.getElementById("wa"),pre=document.getElementById("msgtxt"),prev=document.getElementById("prev");
  if(!(l.length||e)||!sel){pre.textContent=EMPTY;prev.classList.add("empty");wa.setAttribute("aria-disabled","true");wa.href="#";return}
  var dia=dsel.options[dsel.selectedIndex].text;
  var msg="Olá, Sirlene! 💗 Gostaria de reservar um horário no seu estúdio.\n\n"+
    "📅 Dia: "+dia+"\n"+
    "🕐 Horário: "+sel+"\n"+
    "✂️ Procedimento(s): "+l.join(", ")+"\n"+
    (e?"📝 Observações: "+e+"\n":"")+
    "\nEstou ciente do sinal de 50% e de que ele não é devolvido. Pode confirmar, por favor? Obrigada!";
  pre.textContent=msg;prev.classList.remove("empty");
  wa.href=WA+"?text="+encodeURIComponent(msg);
  wa.removeAttribute("aria-disabled");
  wa.onclick=function(){try{navigator.clipboard.writeText(msg)}catch(x){}};
}
document.querySelectorAll("input[type=checkbox]").forEach(function(c){c.onchange=upd});
document.getElementById("extra").oninput=upd;dsel.onchange=upd;
</script>
</body>
</html>
