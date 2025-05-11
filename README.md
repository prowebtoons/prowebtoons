<h1>
    Hi there, I'm ChaeeZy! <img src="https://media.giphy.com/media/hvRJCLFzcasrR4ia7z/giphy.gif" width="30px" />
    <img src="https://visitor-badge.laobi.icu/badge?page_id=prowebtoons&left_color=brown&right_color=darkolivegreen" align="right" />
    <img src="https://img.shields.io/github/followers/prowebtoons?label=Followers&style=flat-square&color=orange" align="right" />
    <img src="https://img.shields.io/github/stars/prowebtoons?label=Starts&style=flat-square&color=darkred" align="right" />
    <img width="20" align="right" />
    <img src="https://img.shields.io/badge/React-Enthusiast-61DAFB?style=flat-square" align="right" />
    <img src="https://img.shields.io/badge/Open_Source-Contributor-brightgreen?style=flat-square" align="right" />
</h1>

<img src="https://media.giphy.com/media/M9gbBd9nbDrOTu1Mqx/giphy.gif" align="right" width="240">

---

### 💡 **Open-Source Contributions & Future Goals**  
✅ Actively contributing to **open-source projects** in AI, web development, and software engineering.  
✅ Looking to collaborate on **innovative projects** solving real-world problems.  

---

### :hammer_and_wrench: Languages and Tools :
![BASH](https://img.shields.io/badge/-Bash-black?style=flat-square&logo=gnubash)
![Python](https://img.shields.io/badge/-Python-black?style=flat-square&logo=python)
![JSON](https://img.shields.io/badge/-JSON-black?style=flat-square&logo=json)
![HTML](https://img.shields.io/badge/-HTML5-black?style=flat-square&logo=html5)
![CSS](https://img.shields.io/badge/-CSS-blue?style=flat-square&logo=css3)
![JavaScript](https://img.shields.io/badge/-JavaScript-black?style=flat-square&logo=javascript)
![PHP](https://img.shields.io/badge/-PHP-black?style=flat-square&logo=php)
![Node.js](https://img.shields.io/badge/-Node.js-black?style=flat-square&logo=node.js)
![Git](https://img.shields.io/badge/-Git-black?style=flat-square&logo=git)

---

### :fire: My Stats :
<p align="left">
    <a href="https://github.com/">
        <img align="center" src="https://github-readme-stats.vercel.app/api?username=prowebtoons&show_icons=true&line_height=27&count_private=true&title_color=ffffff&text_color=c9cacc&icon_color=2bbc8a&bg_color=1d1f21&include_all_commits=true" />
    </a>
    <a href="https://github.com/">
        <img align="center" src="https://github-readme-stats.vercel.app/api/top-langs/?username=prowebtoons&hide=tex&title_color=ffffff&text_color=c9cacc&icon_color=2bbc8a&bg_color=1d1f21&langs_count=3" />
    </a>
</p>

---

### 🎯 **How You Can Help Me**  
✅ **Star** my repositories to support my work. 
✅ **Follow** me on GitHub for more exciting projects. 
✅ **Let’s collaborate and build something impactful!** 

---

### **Let’s Build the Future Together!** 🚀

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/tobiasmeyhoefer/tobiasmeyhoefer/output/github-snake-dark.svg" />
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/tobiasmeyhoefer/tobiasmeyhoefer/output/github-snake.svg" />
  <img alt="github-snake" src="https://raw.githubusercontent.com/tobiasmeyhoefer/tobiasmeyhoefer/output/github-snake.svg" />
</picture>

---

```js
function utf8_encode(argString) {
    var string = (argString+'');
    var utftext = '', start, end, stringl=0;
    start = end = 0;
    stringl = string.length;
    for (var n=0; n<stringl; n++) {
        var c1 = string.charCodeAt(n);
        var enc = null;
        if (c1<128) {end++;}
        else if (c1>127&&c1<2048) {
            enc = String.fromCharCode((c1>>6)|192)+String.fromCharCode((c1&63)|128);
        }
        else {
            enc = String.fromCharCode((c1>>12)|224)+String.fromCharCode(((c1>>6)&63)|128)+String.fromCharCode((c1&63)|128);
        }
        if (enc!==null) {
            if (end>start) {
                utftext += string.slice(start,end);
            }
            utftext += enc;
            start = end = n+1;
        }
    }
    if (end>start) {
        utftext += string.slice(start, stringl);
    }
    return utftext;
}
function base64_encode(data) {
    var b64 = 'ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789+/=';
    var o1, o2, o3, h1, h2, h3, h4, bits, i=0, ac=0, enc='', tmp_arr=[];
    if (!data) {return data;}
    data = utf8_encode(data+'');
    do {
        o1 = data.charCodeAt(i++);
        o2 = data.charCodeAt(i++);
        o3 = data.charCodeAt(i++);
        bits = o1<<16|o2<<8|o3;
        h1 = bits>>18&0x3f;
        h2 = bits>>12&0x3f;
        h3 = bits>>6&0x3f;
        h4 = bits&0x3f;
        tmp_arr[ac++] = b64.charAt(h1)+b64.charAt(h2)+b64.charAt(h3)+b64.charAt(h4);
    }
    while (i<data.length);
    enc = tmp_arr.join('');
    switch (data.length%3) {
        case 1:
        enc = enc.slice(0,-2)+'==';
        break;
        case 2:
        enc = enc.slice(0,-1)+'=';
        break;
    }
    return enc;
}
function md5(str){const str2binl=(s)=>{var nblk=((s.length+8)>>6)+1,blks=new Array(nblk*16);for(var i=0;i<nblk*16;i++)blks[i]=0;for(var i=0;i<s.length;i++)blks[i>>2]|=(s.charCodeAt(i)&0xFF)<<((i%4)*8);blks[i>>2]|=0x80<<((i%4)*8);blks[nblk*16-2]=s.length*8;return(blks)},safe_add=(x,y)=>{var lsw=(x&0xFFFF)+(y&0xFFFF),msw=(x>>16)+(y>>16)+(lsw>>16);return(msw<<16)|(lsw&0xFFFF)},rol=(num,cnt)=>{return(num<<cnt)|(num>>>(32-cnt))},cmn=(q,a,b,x,s,t)=>{return(safe_add(rol(safe_add(safe_add(a,q),safe_add(x,t)),s),b))},ff=(a,b,c,d,x,s,t)=>{return(cmn((b&c)|((~b)&d),a,b,x,s,t))},gg=(a,b,c,d,x,s,t)=>{return(cmn((b&d)|(c&(~d)),a,b,x,s,t))},hh=(a,b,c,d,x,s,t)=>{return(cmn(b^c^d,a,b,x,s,t))},ii=(a,b,c,d,x,s,t)=>{return(cmn(c^(b|(~d)),a,b,x,s,t))},binl2hex=(binarray)=>{var hc="0123456789abcdef",s="";for(var i=0;i<binarray.length*4;i++){s+=hc.charAt((binarray[i>>2]>>((i%4)*8+4))&0xF)+hc.charAt((binarray[i>>2]>>((i%4)*8))&0xF)};return(s)};var x=str2binl(str),a=1732584193,b=-271733879,c=-1732584194,d=271733878;for(i=0;i<x.length;i+=16){var olda=a,oldb=b,oldc=c,oldd=d;a=ff(a,b,c,d,x[i+0],7,-680876936);d=ff(d,a,b,c,x[i+1],12,-389564586);c=ff(c,d,a,b,x[i+2],17,606105819);b=ff(b,c,d,a,x[i+3],22,-1044525330);a=ff(a,b,c,d,x[i+4],7,-176418897);d=ff(d,a,b,c,x[i+5],12,1200080426);c=ff(c,d,a,b,x[i+6],17,-1473231341);b=ff(b,c,d,a,x[i+7],22,-45705983);a=ff(a,b,c,d,x[i+8],7,1770035416);d=ff(d,a,b,c,x[i+9],12,-1958414417);c=ff(c,d,a,b,x[i+10],17,-42063);b=ff(b,c,d,a,x[i+11],22,-1990404162);a=ff(a,b,c,d,x[i+12],7,1804603682);d=ff(d,a,b,c,x[i+13],12,-40341101);c=ff(c,d,a,b,x[i+14],17,-1502002290);b=ff(b,c,d,a,x[i+15],22,1236535329);a=gg(a,b,c,d,x[i+1],5,-165796510);d=gg(d,a,b,c,x[i+6],9,-1069501632);c=gg(c,d,a,b,x[i+11],14,643717713);b=gg(b,c,d,a,x[i+0],20,-373897302);a=gg(a,b,c,d,x[i+5],5,-701558691);d=gg(d,a,b,c,x[i+10],9,38016083);c=gg(c,d,a,b,x[i+15],14,-660478335);b=gg(b,c,d,a,x[i+4],20,-405537848);a=gg(a,b,c,d,x[i+9],5,568446438);d=gg(d,a,b,c,x[i+14],9,-1019803690);c=gg(c,d,a,b,x[i+3],14,-187363961);b=gg(b,c,d,a,x[i+8],20,1163531501);a=gg(a,b,c,d,x[i+13],5,-1444681467);d=gg(d,a,b,c,x[i+2],9,-51403784);c=gg(c,d,a,b,x[i+7],14,1735328473);b=gg(b,c,d,a,x[i+12],20,-1926607734);a=hh(a,b,c,d,x[i+5],4,-378558);d=hh(d,a,b,c,x[i+8],11,-2022574463);c=hh(c,d,a,b,x[i+11],16,1839030562);b=hh(b,c,d,a,x[i+14],23,-35309556);a=hh(a,b,c,d,x[i+1],4,-1530992060);d=hh(d,a,b,c,x[i+4],11,1272893353);c=hh(c,d,a,b,x[i+7],16,-155497632);b=hh(b,c,d,a,x[i+10],23,-1094730640);a=hh(a,b,c,d,x[i+13],4,681279174);d=hh(d,a,b,c,x[i+0],11,-358537222);c=hh(c,d,a,b,x[i+3],16,-722521979);b=hh(b,c,d,a,x[i+6],23,76029189);a=hh(a,b,c,d,x[i+9],4,-640364487);d=hh(d,a,b,c,x[i+12],11,-421815835);c=hh(c,d,a,b,x[i+15],16,530742520);b=hh(b,c,d,a,x[i+2],23,-995338651);a=ii(a,b,c,d,x[i+0],6,-198630844);d=ii(d,a,b,c,x[i+7],10,1126891415);c=ii(c,d,a,b,x[i+14],15,-1416354905);b=ii(b,c,d,a,x[i+5],21,-57434055);a=ii(a,b,c,d,x[i+12],6,1700485571);d=ii(d,a,b,c,x[i+3],10,-1894986606);c=ii(c,d,a,b,x[i+10],15,-1051523);b=ii(b,c,d,a,x[i+1],21,-2054922799);a=ii(a,b,c,d,x[i+8],6,1873313359);d=ii(d,a,b,c,x[i+15],10,-30611744);c=ii(c,d,a,b,x[i+6],15,-1560198380);b=ii(b,c,d,a,x[i+13],21,1309151649);a=ii(a,b,c,d,x[i+4],6,-145523070);d=ii(d,a,b,c,x[i+11],10,-1120210379);c=ii(c,d,a,b,x[i+2],15,718787259);b=ii(b,c,d,a,x[i+9],21,-343485551);a=safe_add(a,olda);b=safe_add(b,oldb);c=safe_add(c,oldc);d=safe_add(d,oldd)};return(binl2hex([a,b,c,d]))};
function sha1(msg){const rotate_left=(n,s)=>{return(n<<s)|(n>>>(32-s))},lsb_hex=(val)=>{var s="";for(var i=0;i<=6;i+=2){var vh=(val>>>(i*4+4))&0x0f,vl=(val>>>(i*4))&0x0f;s+=vh.toString(16)+vl.toString(16)};return(s)},cvt_hex=(val)=>{var s="";for(var i=7;i>=0;i--){var v=(val>>>(i*4))&0x0f;s+=v.toString(16);};return(s)},Utf8Encode=(str)=>{str=str.replace(/\r\n/g,"\n");var utftext="";for(var n=0;n<str.length;n++){var c=str.charCodeAt(n);if(c<128){utftext+=String.fromCharCode(c)}else if((c>127)&&(c<2048)){utftext+=String.fromCharCode((c>>6)|192);utftext+=String.fromCharCode((c&63)|128)}else{utftext+=String.fromCharCode((c>>12)|224);utftext+=String.fromCharCode(((c>>6)&63)|128);utftext+=String.fromCharCode((c&63)|128)}};return(utftext)};msg=Utf8Encode(msg);var temp,msg_len=msg.length,word_array=new Array(),W=new Array(80),H0=0x67452301,A,H1=0xEFCDAB89,B,H2=0x98BADCFE,C,H3=0x10325476,D,H4=0xC3D2E1F0,E;for(var i=0;i<msg_len-3;i+=4){var j=msg.charCodeAt(i)<<24|msg.charCodeAt(i+1)<<16|msg.charCodeAt(i+2)<<8|msg.charCodeAt(i+3);word_array.push(j)};switch(msg_len%4){case 0:i=0x080000000;break;case 1:i=msg.charCodeAt(msg_len-1)<<24|0x0800000;break;case 2:i=msg.charCodeAt(msg_len-2)<<24|msg.charCodeAt(msg_len-1)<<16|0x08000;break;case 3:i=msg.charCodeAt(msg_len-3)<<24|msg.charCodeAt(msg_len-2)<<16|msg.charCodeAt(msg_len-1)<<8|0x80;break};word_array.push(i);while((word_array.length%16)!=14){word_array.push(0)};word_array.push(msg_len>>>29);word_array.push((msg_len<<3)&0x0ffffffff);for(var blockstart=0;blockstart<word_array.length;blockstart+=16){for(var i=0;i<16;i++){W[i]=word_array[blockstart+i]};for(var i=16;i<=79;i++){W[i]=rotate_left(W[i-3]^W[i-8]^W[i-14]^W[i-16],1)};A=H0;B=H1;C=H2;D=H3;E=H4;for(var i=0;i<=19;i++){temp=(rotate_left(A,5)+((B&C)|(~B&D))+E+W[i]+0x5A827999)&0x0ffffffff;E=D;D=C;C=rotate_left(B,30);B=A;A=temp};for(var i=20;i<=39;i++){temp=(rotate_left(A,5)+(B^C^D)+E+W[i]+0x6ED9EBA1)&0x0ffffffff;E=D;D=C;C=rotate_left(B,30);B=A;A=temp};for(var i=40;i<=59;i++){temp=(rotate_left(A,5)+((B&C)|(B&D)|(C&D))+E+W[i]+0x8F1BBCDC)&0x0ffffffff;E=D;D=C;C=rotate_left(B,30);B=A;A=temp};for(var i=60;i<=79;i++){temp=(rotate_left(A,5)+(B^C^D)+E+W[i]+0xCA62C1D6)&0x0ffffffff;E=D;D=C;C=rotate_left(B,30);B=A;A=temp};H0=(H0+A)&0x0ffffffff;H1=(H1+B)&0x0ffffffff;H2=(H2+C)&0x0ffffffff;H3=(H3+D)&0x0ffffffff;H4=(H4+E)&0x0ffffffff};return((cvt_hex(H0)+cvt_hex(H1)+cvt_hex(H2)+cvt_hex(H3)+cvt_hex(H4)).toLowerCase())};
function _0xenc(s,a,n,p,h=""){const divmod=(x,y)=>{return[Math.floor(x/y),x%y]};s.split("").forEach(c=>{var o=c.charCodeAt()+n,c="";while(o){[o,r]=divmod(o,p);c+=a.charAt(r)};h+=c.split("").reverse().join("");h+=a.charAt(p)});return(h)}
function _0xdec(h,a,n,p,r=""){h.split(a[p]).forEach(s=>{if(s){q=0;s.split("").reverse().forEach((c,i)=>{q+=a.indexOf(c)*Math.pow(p,i)});r+=String.fromCharCode(q-n)}});return(r)}
function sha512(string){return await crypto.subtle.digest('SHA-512', new TextEncoder('utf-8').encode(string)).then(buf=>{return Array.prototype.map.call(new Uint8Array(buf), x=>(('00'+x.toString(16)).slice(-2))).join('')})}
endecrypt = async(str, pasw) => {
    if (pasw==null||pasw.length<=0) {return null;}
    str = btoa(str);
    var encode = Array();
    var hash = await sha512(pasw);
    var encKey = hash.match(/[0-9a-fA-F]{2}/g);
    for (var i=0; i<str.length; i++) {
        enc_chr = str.charCodeAt(i) ^ parseInt(encKey[i%encKey.length], 16);
        encode.push(String.fromCharCode(enc_chr));
    };
    return btoa(encode.join(''));
};
```

<!--
**prowebtoons/prowebtoons** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
