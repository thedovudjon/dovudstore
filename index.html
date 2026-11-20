<!DOCTYPE html>
<html lang="ru">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1, viewport-fit=cover">
<title>dovudstore — объявления</title>
<style>
:root{--bg:#f4f5f9;--card:#fff;--tx:#1d2330;--mut:#6b7385;--ac:#e8590c;--acx:#fff;--bd:#e3e6ee;--er:#d93a3a;--ok:#1f9d55;box-sizing:border-box;padding-top:env(safe-area-inset-top,0px);padding-bottom:env(safe-area-inset-bottom,0px)}
@media (prefers-color-scheme:dark){:root:not([data-theme="light"]){--bg:#12141a;--card:#1c1f28;--tx:#eceef4;--mut:#9aa1b2;--ac:#ff8a4c;--acx:#1a1208;--bd:#2b2f3b;--er:#ff6b6b;--ok:#4ade80;color-scheme:dark}}
:root[data-theme="dark"]{--bg:#12141a;--card:#1c1f28;--tx:#eceef4;--mut:#9aa1b2;--ac:#ff8a4c;--acx:#1a1208;--bd:#2b2f3b;--er:#ff6b6b;--ok:#4ade80;color-scheme:dark}
*{box-sizing:border-box}
html{scroll-padding-top:env(safe-area-inset-top,0px)}
body{margin:0;background:var(--bg);color:var(--tx);font:16px/1.5 system-ui,-apple-system,"Segoe UI",Roboto,sans-serif}
header{display:flex;align-items:center;justify-content:space-between;gap:10px;flex-wrap:wrap;padding:12px 20px;background:var(--card);border-bottom:1px solid var(--bd);position:sticky;top:env(safe-area-inset-top,0px);z-index:5}
.logo{font-size:19px;font-weight:800;cursor:pointer;color:var(--ac)}
nav{display:flex;gap:8px;align-items:center;flex-wrap:wrap}
main{max-width:980px;margin:22px auto;padding:0 16px}
.card{background:var(--card);border:1px solid var(--bd);border-radius:14px;padding:20px;margin-bottom:16px}
h2{margin:0 0 14px;font-size:21px}
label{display:block;font-size:14px;color:var(--mut);margin:12px 0 4px}
input,textarea,select{width:100%;padding:10px 12px;border:1px solid var(--bd);border-radius:9px;background:var(--bg);color:var(--tx);font:inherit}
textarea{min-height:90px;resize:vertical}
button{padding:9px 16px;border:0;border-radius:9px;background:var(--ac);color:var(--acx);font:inherit;font-weight:600;cursor:pointer}
button.sec{background:transparent;color:var(--tx);border:1px solid var(--bd)}
button.dng{background:var(--er);color:#fff}
button.sm{padding:5px 10px;font-size:13px}
.link{background:none;border:0;color:var(--ac);padding:0;text-decoration:underline}
.msg{margin-top:12px;font-size:14px;min-height:20px}.er{color:var(--er)}.ok{color:var(--ok)}
.auth{max-width:400px;margin:40px auto}
.row{display:flex;gap:12px;align-items:center;flex-wrap:wrap}
.filters{display:grid;grid-template-columns:2fr 1fr 1fr;gap:10px}
@media(max-width:600px){.filters{grid-template-columns:1fr}}
.grid{display:grid;grid-template-columns:repeat(auto-fill,minmax(210px,1fr));gap:14px}
.item{background:var(--card);border:1px solid var(--bd);border-radius:14px;overflow:hidden;cursor:pointer;transition:transform .15s}
.item:hover{transform:translateY(-3px)}
.pic{position:relative;overflow:hidden;height:150px;display:flex;align-items:center;justify-content:center;font-size:56px;background:var(--bg)}.pic img{width:100%;height:100%;object-fit:cover}.big img{max-width:100%;max-height:340px;border-radius:10px}.ttl{font-weight:600}
.item .b{padding:12px}
.price{font-weight:800;font-size:18px}
.mut{color:var(--mut);font-size:13px}
.tag{display:inline-block;padding:2px 10px;border-radius:99px;font-size:12px;font-weight:600;background:var(--bd);color:var(--mut)}
.tag.a{background:var(--ac);color:var(--acx)}
.big{font-size:90px;text-align:center;background:var(--bg);border-radius:12px;padding:20px}
.tw{overflow-x:auto}
table{width:100%;border-collapse:collapse;font-size:14px}
th,td{text-align:left;padding:9px 8px;border-bottom:1px solid var(--bd);white-space:nowrap}
th{color:var(--mut)}
.stats{display:grid;grid-template-columns:repeat(auto-fit,minmax(140px,1fr));gap:12px;margin-bottom:16px}
.stat{background:var(--card);border:1px solid var(--bd);border-radius:12px;padding:12px}.stat b{font-size:24px;display:block}
</style>
</head>
<body>
<header><span class="logo" onclick="go('home')">🛒 dovudstore</span><nav id="nav"></nav></header>
<main id="app"></main>
<script>
var mem = {};
function load(k,d){try{var v=localStorage.getItem(k);return v?JSON.parse(v):d}catch(e){return k in mem?mem[k]:d}}
function save(k,v){mem[k]=v;try{localStorage.setItem(k,JSON.stringify(v))}catch(e){}}
var users=load('mk_users',[]), items=load('mk_items',[]), session=load('mk_session',null);
var role=null, view=session?'home':'login', cur=null, F={q:'',cat:'',sort:'new'};
var CATS=['Электроника','Транспорт','Недвижимость','Одежда','Дом и сад','Услуги','Другое'];
var ICON={'Электроника':'📱','Транспорт':'🚗','Недвижимость':'🏠','Одежда':'👕','Дом и сад':'🪴','Услуги':'🛠️','Другое':'📦'};

async function hash(pw,salt){var b=await crypto.subtle.digest('SHA-256',new TextEncoder().encode(salt+pw));return Array.from(new Uint8Array(b)).map(function(x){return x.toString(16).padStart(2,'0')}).join('')}
function rnd(){return Array.from(crypto.getRandomValues(new Uint8Array(8))).map(function(b){return b.toString(16).padStart(2,'0')}).join('')}
function esc(s){return String(s==null?'':s).replace(/[&<>"']/g,function(c){return{'&':'&amp;','<':'&lt;','>':'&gt;','"':'&quot;',"'":'&#39;'}[c]})}
function $(i){return document.getElementById(i)}
function say(t,c){var m=$('msg');if(m){m.className='msg '+(c||'');m.textContent=t}}
function me(){return users.find(function(u){return u.id===session})||null}
function uname(id){var u=users.find(function(x){return x.id===id});return u?u.name:'Удалён'}
function money(i){return Number(i.price).toLocaleString('ru-RU')+' '+i.cur}
function date(t){return new Date(t).toLocaleDateString('ru-RU')}
async function addUser(l,p,role,n,e){var s=rnd();var u={id:rnd(),login:l,name:n||l,email:e||l,role:role,salt:s,hash:await hash(p,s),created:Date.now(),last:Date.now()};users.push(u);save('mk_users',users);return u}

function render(){
  var u=me(),nav=$('nav');
  if(session&&(!u||u.banned)){session=null;save('mk_session',null);u=null}
  if(!users.length&&role!=='user'){nav.innerHTML='';return role==='admin'?setup():choose()}
  nav.innerHTML=(u?'<button class="sm" onclick="go(\'new\')">+ Подать объявление</button><button class="sec sm" onclick="go(\'profile\')">👤 Профиль</button>'+(u.role==='admin'?'<button class="sec sm" onclick="go(\'admin\')">Админ</button>':'')+'<button class="sec sm" onclick="logout()">Выйти</button>':'<button class="sec sm" onclick="role=null;go(\'login\')">Войти</button><button class="sm" onclick="role=\'user\';go(\'login\');loginScr(true)">Регистрация</button>');
  if(view==='home')return home();
  if(view==='item')return detail();
  if(view==='login')return role?loginScr(false):choose();
  if(!u){view='login';return role?loginScr(false):choose()}
  if(view==='new')return form();
  if(view==='profile')return profile();
  if(view==='admin'&&u.role==='admin')return admin();
  view='home';home();
}
function go(v,id){view=v;cur=id||null;render();window.scrollTo(0,0)}
function logout(){session=null;role=null;save('mk_session',null);go('login')}

function setup(){
  $('app').innerHTML='<div class="card auth"><h2>Первый запуск</h2><p class="mut">Создайте аккаунт администратора площадки.</p><label>Email</label><input id="l" type="email" autocomplete="email"><label>Имя</label><input id="n"><label>Пароль (от 8 символов)</label><input id="p" type="password"><div style="margin-top:14px"><button onclick="doSetup()">Создать администратора</button></div><div id="msg" class="msg"></div></div>';
}
async function doSetup(){
  var l=$('l').value.trim(),p=$('p').value;
  l=l.toLowerCase();if(!/^[^\s@]+@[^\s@]+\.[^\s@]+$/.test(l))return say('Введите корректный email','er');
  if(p.length<8)return say('Пароль — минимум 8 символов','er');
  var u=await addUser(l,p,'admin',$('n').value.trim());
  [['Смартфон в хорошем состоянии','Электроника',1800,'TJS','Душанбе','Почти новый, полный комплект, есть чек.'],['Велосипед горный','Транспорт',350,'USD','Худжанд','Алюминиевая рама, 21 скорость.'],['Диван угловой','Дом и сад',2500,'TJS','Душанбе','Самовывоз, обивка в отличном состоянии.']].forEach(function(d){
    items.push({id:rnd(),title:d[0],cat:d[1],price:d[2],cur:d[3],city:d[4],desc:d[5],contact:'Демо-объявление',owner:u.id,created:Date.now()})});
  save('mk_items',items);session=u.id;save('mk_session',session);go('home');
}

function choose(){$('app').innerHTML='<div style="max-width:560px;margin:30px auto;text-align:center"><h2>🛒 Добро пожаловать в dovudstore</h2><p class="mut">Выберите, как войти</p><div class="grid" style="grid-template-columns:repeat(auto-fit,minmax(220px,1fr))"><div class="item" style="padding:24px" onclick="pick(\'user\')"><div style="font-size:48px">👤</div><h2>Я пользователь</h2><div class="mut">Смотреть и подавать объявления</div></div><div class="item" style="padding:24px" onclick="pick(\'admin\')"><div style="font-size:48px">🛡️</div><h2>Я администратор</h2><div class="mut">Управление сайтом</div></div></div><p><button class="link" onclick="go(\'home\')">Просто смотреть объявления</button></p></div>'}
function pick(r){role=r;if(r==='admin'&&!users.some(function(u){return u.role==='admin'}))return setup();loginScr(false)}
function loginScr(reg){
  $('app').innerHTML='<div class="card auth"><h2>'+(reg?'Регистрация':role==='admin'?'Вход администратора':'Вход')+'</h2><label>Email</label><input id="l" type="email" autocomplete="email">'+(reg?'<label>Имя</label><input id="n">':'')+'<label>Пароль</label><input id="p" type="password"><div class="row" style="margin-top:14px"><button onclick="'+(reg?'doReg()':'doLogin()')+'">'+(reg?'Создать аккаунт':'Войти')+'</button>'+(role==='admin'?'':'<button class="link" onclick="loginScr('+(!reg)+')">'+(reg?'Уже есть аккаунт':'Регистрация')+'</button>')+'</div><div id="msg" class="msg"></div></div>';
  $('p').addEventListener('keydown',function(e){if(e.key==='Enter')reg?doReg():doLogin()});
}
async function doLogin(){
  var l=$('l').value.trim(),u=users.find(function(x){return x.login.toLowerCase()===l.toLowerCase()});
  if(!u||(await hash($('p').value,u.salt))!==u.hash)return say('Неверный логин или пароль','er');
  if(u.banned)return say('Аккаунт заблокирован администратором','er');
  if(role==='admin'&&u.role!=='admin')return say('Этот аккаунт не является администратором','er');
  u.last=Date.now();save('mk_users',users);session=u.id;save('mk_session',session);go(u.role==='admin'?'admin':'home');
}
async function doReg(){
  var l=$('l').value.trim(),p=$('p').value;
  l=l.toLowerCase();if(!/^[^\s@]+@[^\s@]+\.[^\s@]+$/.test(l))return say('Введите корректный email','er');
  if(p.length<8)return say('Пароль — минимум 8 символов','er');
  if(users.some(function(x){return x.login.toLowerCase()===l.toLowerCase()}))return say('Этот email уже зарегистрирован','er');
  var u=await addUser(l,p,'user',$('n').value.trim());
  session=u.id;save('mk_session',session);go('home');
}

function home(){
  var cats='<option value="">Все категории</option>'+CATS.map(function(c){return'<option'+(F.cat===c?' selected':'')+'>'+c+'</option>'}).join('');
  $('app').innerHTML='<div class="card"><div class="filters"><input id="q" placeholder="Поиск по объявлениям…" value="'+esc(F.q)+'"><select id="c">'+cats+'</select><select id="s"><option value="new">Сначала новые</option><option value="lo"'+(F.sort==='lo'?' selected':'')+'>Дешевле</option><option value="hi"'+(F.sort==='hi'?' selected':'')+'>Дороже</option></select></div></div><div id="list"></div>';
  $('q').oninput=function(){F.q=this.value;list()};$('c').onchange=function(){F.cat=this.value;list()};$('s').onchange=function(){F.sort=this.value;list()};
  list();
}
function pic(i){return i.img?'<img src="'+i.img+'" alt="">':ICON[i.cat]}
function card(i){return'<div class="item" onclick="go(\'item\',\''+i.id+'\')"><div class="pic">'+pic(i)+'<span class="tag a" style="position:absolute;top:8px;left:8px">'+esc(i.cond||'Б/у')+'</span></div><div class="b"><div class="price">'+esc(money(i))+'</div><div class="ttl">'+esc(i.title)+'</div><div class="mut">'+esc(i.city)+' · '+date(i.created)+'</div><div class="mut">'+esc(i.cat)+' · '+esc(uname(i.owner))+'</div></div></div>'}
function list(){
  var q=F.q.toLowerCase(),r=items.filter(function(i){return(!F.cat||i.cat===F.cat)&&(!q||(i.title+' '+i.desc+' '+i.city).toLowerCase().indexOf(q)>-1)});
  r.sort(function(a,b){return F.sort==='lo'?a.price-b.price:F.sort==='hi'?b.price-a.price:b.created-a.created});
  $('list').innerHTML=r.length?'<div class="grid">'+r.map(card).join('')+'</div>':'<div class="card mut" style="text-align:center">Ничего не найдено. Подайте первое объявление!</div>';
}
function detail(){
  var i=items.find(function(x){return x.id===cur});
  if(!i)return go('home');
  var u=me(),can=u&&(u.id===i.owner||u.role==='admin');
  $('app').innerHTML='<button class="sec sm" onclick="go(\'home\')">← Назад</button><div class="card" style="margin-top:12px"><div class="big">'+pic(i)+'</div><h2 style="margin-top:16px">'+esc(i.title)+'</h2><div class="price" style="font-size:26px">'+esc(money(i))+'</div><p><span class="tag a">'+esc(i.cat)+'</span> <span class="tag">'+esc(i.cond||'Б/у')+'</span> <span class="tag">'+esc(i.city)+'</span> <span class="tag">'+date(i.created)+'</span></p><p style="white-space:pre-wrap">'+esc(i.desc)+'</p><div class="mut">Продавец: '+esc(uname(i.owner))+'</div><div style="margin:12px 0"><b>Контакты:</b> '+esc(i.contact)+'</div>'+(can?'<button class="dng sm" onclick="delItem(\''+i.id+'\',\'home\')">Удалить объявление</button>':'')+'</div>';
}
function form(){
  $('app').innerHTML='<div class="card" style="max-width:560px;margin:auto"><h2>Новое объявление</h2><label>Заголовок</label><input id="t" maxlength="80"><label>Категория</label><select id="c">'+CATS.map(function(c){return'<option>'+c+'</option>'}).join('')+'</select><div class="row"><div style="flex:2"><label>Цена</label><input id="pr" type="number" min="0"></div><div style="flex:1"><label>Валюта</label><select id="cu"><option>TJS</option><option>USD</option><option>RUB</option></select></div></div><label>Состояние</label><select id="cd"><option>Новое</option><option>Б/у</option></select><label>Фото (необязательно)</label><input id="ph" type="file" accept="image/*"><label>Город</label><input id="ci"><label>Описание</label><textarea id="d"></textarea><label>Контакты (телефон, Telegram)</label><input id="co"><div style="margin-top:14px"><button onclick="addItem()">Опубликовать</button></div><div id="msg" class="msg"></div></div>';
}
function shrink(f){return new Promise(function(ok){if(!f)return ok('');var r=new FileReader();r.onload=function(){var im=new Image();im.onload=function(){var s=Math.min(1,500/Math.max(im.width,im.height)),c=document.createElement('canvas');c.width=im.width*s;c.height=im.height*s;c.getContext('2d').drawImage(im,0,0,c.width,c.height);ok(c.toDataURL('image/jpeg',.75))};im.onerror=function(){ok('')};im.src=r.result};r.onerror=function(){ok('')};r.readAsDataURL(f)})}
async function addItem(){
  var t=$('t').value.trim(),pr=parseFloat($('pr').value);
  if(t.length<3)return say('Введите заголовок','er');
  if(isNaN(pr)||pr<0)return say('Укажите цену','er');
  if(!$('co').value.trim())return say('Укажите контакты','er');
  var img=await shrink($('ph').files[0]);items.push({id:rnd(),img:img,cond:$('cd').value,title:t,cat:$('c').value,price:pr,cur:$('cu').value,city:$('ci').value.trim()||'—',desc:$('d').value.trim(),contact:$('co').value.trim(),owner:session,created:Date.now()});
  save('mk_items',items);go('home');
}
function delItem(id,to){if(!confirm('Удалить объявление?'))return;items=items.filter(function(x){return x.id!==id});save('mk_items',items);go(to)}

function profile(){
  var u=me(),mine=items.filter(function(i){return i.owner===u.id});
  $('app').innerHTML='<div class="card"><h2>'+esc(u.name)+' <span class="tag '+(u.role==='admin'?'a':'')+'">'+(u.role==='admin'?'Администратор':'Пользователь')+'</span></h2><div class="mut">'+esc(u.email||u.login)+' · с '+date(u.created)+'</div><div class="row" style="margin-top:12px"><input id="n" value="'+esc(u.name)+'" style="max-width:260px"><button class="sec sm" onclick="saveName()">Сменить имя</button></div></div>'+
  '<div class="card"><h2>Мои объявления ('+mine.length+')</h2>'+(mine.length?'<div class="tw"><table>'+mine.map(function(i){return'<tr><td>'+esc(i.title)+'</td><td>'+esc(money(i))+'</td><td><button class="sec sm" onclick="go(\'item\',\''+i.id+'\')">Открыть</button> <button class="dng sm" onclick="delItem(\''+i.id+'\',\'profile\')">Удалить</button></td></tr>'}).join('')+'</table></div>':'<span class="mut">Пока пусто.</span>')+'</div>'+
  '<div class="card"><h2>Смена пароля</h2><input id="op" type="password" placeholder="Текущий пароль"><br><br><input id="np" type="password" placeholder="Новый пароль (от 8 символов)"><div style="margin-top:12px"><button class="sec" onclick="changePw()">Изменить</button></div><div id="msg" class="msg"></div></div>';
}
function saveName(){var u=me();u.name=$('n').value.trim()||u.login;save('mk_users',users);profile()}
async function changePw(){
  var u=me(),np=$('np').value;
  if((await hash($('op').value,u.salt))!==u.hash)return say('Текущий пароль неверный','er');
  if(np.length<8)return say('Новый пароль слишком короткий','er');
  u.salt=rnd();u.hash=await hash(np,u.salt);save('mk_users',users);say('Пароль изменён','ok');
}

var UQ='';
function admin(){
  var ad=users.filter(u=>u.role==='admin').length,bl=users.filter(u=>u.banned).length;
  $('app').innerHTML='<div class="stats"><div class="stat"><b>'+users.length+'</b>Профилей</div><div class="stat"><b>'+ad+'</b>Админов</div><div class="stat"><b>'+bl+'</b>Заблокировано</div><div class="stat"><b>'+items.length+'</b>Объявлений</div></div>'+
  '<div class="card"><h2>Все профили</h2><input id="uq" placeholder="Поиск по имени или email…" value="'+esc(UQ)+'" oninput="UQ=this.value;utable()"><div class="tw" id="ut" style="margin-top:12px"></div></div>'+
  '<div class="card"><h2>Добавить профиль</h2><div class="row"><input id="an" placeholder="Имя" style="flex:1"><input id="ae" type="email" placeholder="Email" style="flex:1"><input id="ap" type="password" placeholder="Пароль (от 8)" style="flex:1"></div><div class="row" style="margin-top:10px"><select id="ar" style="max-width:200px"><option value="user">Пользователь</option><option value="admin">Администратор</option></select><button onclick="adminAdd()">Создать</button></div><div id="msg" class="msg"></div></div>'+
  '<div class="card"><h2>Модерация объявлений</h2><div class="tw"><table><tr><th>Заголовок</th><th>Цена</th><th>Автор</th><th></th></tr>'+items.map(i=>'<tr><td>'+esc(i.title)+'</td><td>'+esc(money(i))+'</td><td>'+esc(uname(i.owner))+'</td><td><button class="dng sm" onclick="delItem(\'' +i.id+'\',\'admin\')">Удалить</button></td></tr>').join('')+'</table></div></div>';
  utable();
}
function utable(){
  var q=UQ.toLowerCase();
  $('ut').innerHTML='<table><tr><th>Email</th><th>Имя</th><th>Статус</th><th>Объявл.</th><th>Регистрация</th><th></th></tr>'+users.filter(u=>!q||(u.login+' '+u.name+' '+u.email).toLowerCase().indexOf(q)>-1).map(u=>'<tr><td>'+esc(u.email||u.login)+'</td><td>'+esc(u.name)+'</td><td><span class="tag '+(u.role==='admin'?'a':'')+'">'+(u.role==='admin'?'админ':'user')+'</span>'+(u.banned?' <span class="tag" style="color:var(--er)">блок</span>':'')+'</td><td>'+items.filter(i=>i.owner===u.id).length+'</td><td>'+date(u.created)+'</td><td><button class="sec sm" onclick="userView(\''+u.id+'\')">Открыть</button></td></tr>').join('')+'</table>';
}
async function adminAdd(){
  var n=$('an').value.trim(),e=$('ae').value.trim().toLowerCase(),p=$('ap').value;
  if(!/^[^\s@]+@[^\s@]+\.[^\s@]+$/.test(e))return say('Введите корректный email','er');
  if(p.length<8)return say('Пароль — минимум 8 символов','er');
  if(users.some(x=>x.login.toLowerCase()===e))return say('Этот email уже зарегистрирован','er');
  await addUser(e,p,$('ar').value,n);admin();say('Профиль создан','ok');
}
function userView(id){
  var u=users.find(x=>x.id===id),self=id===session,mine=items.filter(i=>i.owner===id);
  $('app').innerHTML='<button class="sec sm" onclick="go(\'admin\')">← К списку</button><div class="card" style="margin-top:12px"><h2>'+esc(u.name)+' <span class="tag '+(u.role==='admin'?'a':'')+'">'+(u.role==='admin'?'Администратор':'Пользователь')+'</span>'+(u.banned?' <span class="tag" style="color:var(--er)">заблокирован</span>':'')+'</h2><div class="mut">Регистрация: '+date(u.created)+(self?' · это ваш профиль':'')+'</div><label>Имя</label><input id="un" value="'+esc(u.name)+'"><label>Email</label><input id="ue" value="'+esc(u.email||u.login)+'"><label>Роль</label><select id="ur"'+(self?' disabled':'')+'><option value="user"'+(u.role==='user'?' selected':'')+'>Пользователь</option><option value="admin"'+(u.role==='admin'?' selected':'')+'>Администратор</option></select><div class="row" style="margin-top:14px"><button onclick="saveUser(\''+id+'\')">Сохранить</button>'+(self?'':'<button class="sec" onclick="banUser(\''+id+'\')">'+(u.banned?'Разблокировать':'Заблокировать')+'</button><button class="sec" onclick="resetPw(\''+id+'\')">Сбросить пароль</button><button class="dng" onclick="delUser(\''+id+'\')">Удалить профиль</button>')+'</div><div id="msg" class="msg"></div></div><div class="card"><h2>Объявления ('+mine.length+')</h2>'+(mine.length?'<div class="grid">'+mine.map(card).join('')+'</div>':'<span class="mut">Нет объявлений.</span>')+'</div>';
}
function saveUser(id){
  var u=users.find(x=>x.id===id),e=$('ue').value.trim().toLowerCase();
  if(!/^[^\s@]+@[^\s@]+\.[^\s@]+$/.test(e))return say('Введите корректный email','er');
  if(users.some(x=>x.id!==id&&x.login.toLowerCase()===e))return say('Этот email занят','er');
  u.name=$('un').value.trim()||e;u.email=e;u.login=e;
  if(id!==session)u.role=$('ur').value;
  save('mk_users',users);userView(id);say('Сохранено','ok');
}
function banUser(id){var u=users.find(x=>x.id===id);u.banned=!u.banned;save('mk_users',users);userView(id);say(u.banned?'Профиль заблокирован':'Профиль разблокирован','ok')}
async function resetPw(id){
  var u=users.find(x=>x.id===id),p=prompt('Новый пароль для '+(u.email||u.login)+' (от 8 символов):');
  if(!p)return;if(p.length<8)return say('Пароль слишком короткий','er');
  u.salt=rnd();u.hash=await hash(p,u.salt);save('mk_users',users);say('Пароль изменён','ok');
}
function adminOld(){
  var cu=me(),ad=users.filter(function(u){return u.role==='admin'}).length;
  $('app').innerHTML='<div class="stats"><div class="stat"><b>'+users.length+'</b>Пользователей</div><div class="stat"><b>'+ad+'</b>Админов</div><div class="stat"><b>'+items.length+'</b>Объявлений</div></div>'+
  '<div class="card"><h2>Пользователи</h2><div class="tw"><table><tr><th>Email</th><th>Имя</th><th>Роль</th><th>Действия</th></tr>'+users.map(function(u){return'<tr><td>'+esc(u.login)+'</td><td>'+esc(u.name)+'</td><td>'+u.role+'</td><td>'+(u.id===cu.id?'<i class="mut">это вы</i>':'<button class="sec sm" onclick="toggleRole(\''+u.id+'\')">'+(u.role==='admin'?'→ user':'→ admin')+'</button> <button class="dng sm" onclick="delUser(\''+u.id+'\')">Удалить</button>')+'</td></tr>'}).join('')+'</table></div></div>'+
  '<div class="card"><h2>Модерация объявлений</h2><div class="tw"><table><tr><th>Заголовок</th><th>Цена</th><th>Автор</th><th></th></tr>'+items.map(function(i){return'<tr><td>'+esc(i.title)+'</td><td>'+esc(money(i))+'</td><td>'+esc(uname(i.owner))+'</td><td><button class="dng sm" onclick="delItem(\''+i.id+'\',\'admin\')">Удалить</button></td></tr>'}).join('')+'</table></div></div>';
}
function toggleRole(id){var u=users.find(function(x){return x.id===id});u.role=u.role==='admin'?'user':'admin';save('mk_users',users);admin()}
function delUser(id){var u=users.find(function(x){return x.id===id});if(!confirm('Удалить «'+u.login+'» и все его объявления?'))return;users=users.filter(function(x){return x.id!==id});items=items.filter(function(x){return x.owner!==id});save('mk_users',users);save('mk_items',items);admin()}

render();
</script>
</body>
</html>
