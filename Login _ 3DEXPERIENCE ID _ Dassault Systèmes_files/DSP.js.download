define("UWA/Internal/Polyfill/NativeObjects",[],function(){"use strict";var t=Function("return this")();if(!t.UWA_SKIP_POLYFILLS){var e,r,n,o,i,c,a,l,p,u=Function.prototype.call,f=Object.prototype,s=Array.prototype,h=Object("a"),y="a"!==h[0]||!(0 in h);Function.prototype.bind||(Function.prototype.bind=function(t){var e,r,n=this,o=Array.prototype.slice,i=function(){};if("function"!=typeof n)throw new TypeError("Function.prototype.bind called on incompatible "+n);return e=o.call(arguments,1),r=function(){var i;return this instanceof r?(i=n.apply(this,e.concat(o.call(arguments))),i=Object(i)===i?i:this):i=n.apply(t,e.concat(o.call(arguments))),i},n.prototype&&(i.prototype=n.prototype,r.prototype=new i,i.prototype=null),r}),n="\t\n\v\f\r   ᠎             　\u2028\u2029\ufeff",String.prototype.trim&&!n.trim()||(n="["+n+"]",e=new RegExp("^"+n+n+"*"),r=new RegExp(n+n+"*$"),String.prototype.trim=function(){if(null==this)throw new TypeError("can't convert "+this+" to object");return String(this).replace(e,"").replace(r,"")}),i=String.prototype.split,2!=="ab".split(/(?:ab)*/).length||4!==".".split(/(.?)(.?)/).length||"t"==="tesst".split(/(s)*/)[1]||0==="".split(/.?/).length||".".split(/()()/).length>1?(o=void 0===/()??/.exec("")[1],String.prototype.split=function(t,e){var r,n,c,a,l,p,u,f=this;function s(){var t;for(t=1;t<arguments.length-2;t++)void 0===arguments[t]&&(l[t]=void 0)}if(void 0===t&&0===e)r=[];else if("[object RegExp]"!==x(t))r=i.apply(f,[t,e]);else{for(r=[],n=(t.ignoreCase?"i":"")+(t.multiline?"m":"")+(t.extended?"x":"")+(t.sticky?"y":""),c=0,t=new RegExp(t.source,n+"g"),f=String(f),o||(a=new RegExp("^"+t.source+"$(?!\\s)",n)),e=void 0===e?-1>>>0:e>>>0;(l=t.exec(f))&&!((p=l.index+l[0].length)>c&&(r.push(f.slice(c,l.index)),!o&&l.length>1&&l[0].replace(a,s),l.length>1&&l.index<f.length&&Array.prototype.push.apply(r,l.slice(1)),u=l[0].length,c=p,r.length>=e));)t.lastIndex===l.index&&t.lastIndex++;c===f.length?!u&&t.test("")||r.push(""):r.push(f.slice(c)),r=r.length>e?r.slice(0,e):r}return r}):"0".split(void 0,0).length&&(String.prototype.split=function(t,e){return void 0===t&&0===e?[]:i.apply(this,[t,e])}),function(){if("".substr&&"b"!=="0b".substr(-1)){var t=String.prototype.substr;String.prototype.substr=function(e,r){return t.call(this,e<0&&(e=this.length+e)<0?0:e,r)}}}(),String.prototype.repeat||(String.prototype.repeat=(c=function(t,e){var r;return e<1?r="":e%2?r=c(t,e-1)+t:(r=c(t,e/2),r+=r),r},function(t){var e=String(P(this));if((t=E(t))<0||t===1/0)throw new RangeError("Invalid String#repeat value");return c(e,t)})),String.prototype.startsWith||(String.prototype.startsWith=function(t){var e,r,n=String(P(this));if("[object RegExp]"===x(t))throw new TypeError('Cannot call method "startsWith" with a regex');return t=String(t),e=arguments.length>1?arguments[1]:void 0,r=Math.max(E(e),0),n.slice(r,r+t.length)===t}),String.prototype.endsWith||(String.prototype.endsWith=function(t){var e,r,n,o,i=String(P(this));if("[object RegExp]"===x(t))throw new TypeError('Cannot call method "endsWith" with a regex');return t=String(t),e=i.length,n=void 0===(r=arguments.length>1?arguments[1]:void 0)?e:E(r),o=Math.min(Math.max(n,0),e),i.slice(o-t.length,o)===t}),String.prototype.codePointAt||(String.prototype.codePointAt=function(t){var e,r,n=String(P(this)),o=n.length,i=E(t);if(!(i<0||i>=o))return(e=n.charCodeAt(i))<55296||e>56319||i+1===o?e:(r=n.charCodeAt(i+1))<56320||r>57343?e:1024*(e-55296)+(r-56320)+65536}),String.prototype.includes||(String.prototype.includes=function(t,e){return"number"!=typeof e&&(e=0),!(e+t.length>this.length)&&-1!==this.indexOf(t,e)}),Array.isArray||(Array.isArray=function(t){return"[object Array]"===x(t)}),2!==[1,2].splice(0).length&&(a=s.splice,l=s.slice,s.splice=function(t,e){var r=[],n=l.call(arguments);return n.length&&(n[0]=void 0===t?0:t,n[1]=void 0===e?this.length-t:e,r=a.apply(this,n)),r}),1!==[].unshift(0)&&(p=s.unshift,s.unshift=function(){return p.apply(this,arguments),this.length}),s.indexOf&&-1===[0,1].indexOf(1,2)||(s.indexOf=function(t,e){var r=0,n=m(this),o=n.length>>>0;if(!o)return-1;for(arguments.length>1&&(r=E(e)),r=r>=0?r:Math.max(0,o+r);r<o;r++)if(T(n,r)&&n[r]===t)return r;return-1}),s.lastIndexOf&&-1===[0,1].lastIndexOf(0,-3)||(s.lastIndexOf=function(t,e){var r=m(this),n=r.length>>>0,o=n-1;if(!n)return-1;for(arguments.length>1&&(o=Math.min(o,E(e))),o=o>=0?o:n-Math.abs(o);o>=0;o--)if(T(r,o)&&t===r[o])return o;return-1}),s.every||(s.every=function(t,e){var r,n=m(this),o=n.length>>>0;if("function"!=typeof t)throw new TypeError(t+" is not a function");for(r=0;r<o;r++)if(T(n,r)&&!t.call(e,n[r],r,n))return!1;return!0}),s.some||(s.some=function(t,e){var r,n=m(this),o=n.length>>>0;if("function"!=typeof t)throw new TypeError(t+" is not a function");for(r=0;r<o;r++)if(T(n,r)&&t.call(e,n[r],r,n))return!0;return!1}),s.forEach||(s.forEach=function(t,e){var r=0,n=m(this),o=n.length>>>0;if("function"!=typeof t)throw new TypeError(t+" is not a function");for(;r<o;)T(n,r)&&t.call(e,n[r],r,this),r++}),s.map||(s.map=function(t,e){var r,n=m(this),o=n.length>>>0,i=Array(o);if("function"!=typeof t)throw new TypeError(t+" is not a function");for(r=0;r<o;r++)T(n,r)&&(i[r]=t.call(e,n[r],r,n));return i}),s.filter||(s.filter=function(t,e){var r,n,o=m(this),i=o.length>>>0,c=[];if("function"!=typeof t)throw new TypeError(t+" is not a function");for(r=0;r<i;r++)T(o,r)&&(n=o[r],t.call(e,n,r,o)&&c.push(n));return c}),s.reduce||(s.reduce=function(t){var e,r=0,n=m(this),o=n.length>>>0;if("function"!=typeof t)throw new TypeError(t+" is not a function");if(!o&&1===arguments.length)throw new TypeError("reduce of empty array with no initial value");if(arguments.length>=2)e=arguments[1];else for(;;){if(T(n,r)){e=n[r++];break}if(++r>=o)throw new TypeError("reduce of empty array with no initial value")}for(;r<o;r++)T(n,r)&&(e=t(e,n[r],r,n));return e}),s.reduceRight||(s.reduceRight=function(t){var e,r=m(this),n=r.length>>>0,o=n-1;if("function"!=typeof t)throw new TypeError(t+" is not a function");if(!n&&1===arguments.length)throw new TypeError("reduceRight of empty array with no initial value");if(arguments.length>=2)e=arguments[1];else for(;;){if(T(r,o)){e=r[o--];break}if(--o<0)throw new TypeError("reduceRight of empty array with no initial value")}do{T(r,o)&&(e=t(e,r[o],o,r))}while(o--);return e}),s.includes||(s.includes=function(t,e){if(null===this)throw new TypeError('"this" is null or not defined');var r=Object(this),n=r.length>>>0;if(0===n)return!1;for(var o=0|e,i=Math.max(o>=0?o:n-Math.abs(o),0);i<n;){if(r[i]===t)return!0;i++}return!1});var g,b,d,w,O,j=u.bind(f.hasOwnProperty),v=function(t){var e=typeof t;return("object"===e||"function"===e)&&null!==t};if((O=j(f,"__defineGetter__"))&&(g=u.bind(f.__defineGetter__),b=u.bind(f.__defineSetter__),d=u.bind(f.__lookupGetter__),w=u.bind(f.__lookupSetter__)),Object.assign||(Object.assign=function(t){var e,r=m(t);if(1===arguments.length)return r;for(e=1;e<arguments.length;e++){var n=arguments[e];if(null!=n){var o,i=m(n),c=Object.getOwnPropertyNames(i);for(o=0;o<c.length;o++)r[c[o]]=i[c[o]]}}return r}),Object.is||(Object.is=function(t,e){return t===e?0!==t||1/t==1/e:t!=t&&e!=e}),Object.setPrototypeOf||(Object.setPrototypeOf=function(){var t;function e(e,r){return function(t,e){if("function"!=typeof t&&"object"!=typeof t||null===t)throw new TypeError("can not set prototype on a non-object");if("function"!=typeof e&&"object"!=typeof e&&null!==e)throw new TypeError("can only set prototype to an object or null")}(e,r),t.call(e,r),e}try{(t=Object.getOwnPropertyDescriptor(f,"__proto__").set).call({},null)}catch(r){if(f!=={}.__proto__)return;t=function(t){this.__proto__=t},e.polyfill=e(e({},null),f)instanceof Object}return e}()),Object.getPrototypeOf||(Object.getPrototypeOf=function(t){return t.__proto__||(t.constructor?t.constructor.prototype:f)}),Object.getOwnPropertyDescriptor||(Object.getOwnPropertyDescriptor=function(t,e){var r,n,o,i;if(!v(t))throw new TypeError("Object.getOwnPropertyDescriptor called on a non-object:"+t);if(j(t,e))return n={enumerable:!0,configurable:!0},O&&(r=t.__proto__,t.__proto__=f,o=d(t,e),i=w(t,e),t.__proto__=r,o||i)?(o&&(n.get=o),i&&(n.set=i),n):(n.value=t[e],n)}),Object.getOwnPropertyNames||(Object.getOwnPropertyNames=function(t){if(!v(t))throw new TypeError("Object.getOwnPropertyNames called on a non-object:"+t);return Object.keys(t)}),Object.create||(Object.create=function(t,e){var r,n=function(){};return null===t?r={__proto__:null}:(n.prototype=t,(r=new n).__proto__=t),void 0!==e&&Object.defineProperties(r,e),r}),function(){function e(t){try{return Object.defineProperty(t,"sentinel",{}),t.hasOwnProperty("sentinel")}catch(t){}}var r=Object.defineProperty,n=r&&e({}),o=r&&void 0===t.document||e(t.document.createElement("div")),i=r&&!n||!o&&Object.defineProperty;r&&!i||(Object.defineProperty=function(t,e,r){var n;if(!v(t))throw new TypeError("Object.defineProperty called on non-object: "+t);if(!v(r))throw new TypeError("Property description must be an object: "+r);if(i)try{return i.call(Object,t,e,r)}catch(t){}if(j(r,"value"))O&&(d(t,e)||w(t,e))?(n=t.__proto__,t.__proto__=f,delete t[e],t[e]=r.value,t.__proto__=n):t[e]=r.value;else{if(!O)throw new TypeError("getters & setters can not be defined on this javascript engine");j(r,"get")&&g(t,e,r.get),j(r,"set")&&b(t,e,r.set)}return t})}(),Object.defineProperties||(Object.defineProperties=function(t,e){if(!v(t))throw new TypeError("Object.defineProperties called on a non-object");var r;for(r in e)j(e,r)&&Object.defineProperty(t,r,e[r]);return t}),Object.seal||(Object.seal=function(t){if(!v(t))throw new TypeError("Object.seal called on a non-object");return t}),Object.freeze||(Object.freeze=function(t){if(!v(t))throw new TypeError("Object.freeze called on a non-object");return t}),Object.preventExtensions||(Object.preventExtensions=function(t){if(!v(t))throw new TypeError("Object.preventExtensions called on a non-object");return t}),Object.isSealed||(Object.isSealed=function(t){if(!v(t))throw new TypeError("Object.isSealed called on a non-object");return!1}),Object.isFrozen||(Object.isFrozen=function(t){if(!v(t))throw new TypeError("Object.isFrozen called on a non-object");return!1}),Object.isExtensible)try{Object.isExtensible(42)}catch(t){var _=Object.isExtensible;Object.isExtensible=function(t){try{return _(t)}catch(t){return!1}}}else Object.isExtensible=function(t){var e,r;if(!v(t))return!1;for(r="";j(t,r);)r+="?";return t[r]=!0,e=j(t,r),delete t[r],e};Object.keys||(Object.keys=function(t){if(!v(t))throw new TypeError("Object.keys called on a non-object");var e,r,n,o,i=[],c=!j({toString:null},"toString"),a=["toString","toLocaleString","valueOf","hasOwnProperty","isPrototypeOf","propertyIsEnumerable","constructor"],l=a.length;for(n in t)j(t,n)&&i.push(n);if(c)for(e=0,r=l;e<r;e++)j(t,o=a[e])&&i.push(o);return i}),Date.now||(Date.now=function(){return(new Date).getTime()}),Date=function(t){var e,r=[0,31,59,90,120,151,181,212,243,273,304,334,365],n=new RegExp("^(\\d{4}|[-+]\\d{6})(?:-(\\d{2})(?:-(\\d{2})(?:T(\\d{2}):(\\d{2})(?::(\\d{2})(?:(\\.\\d{1,}))?)?(Z|(?:([-+])(\\d{2}):(\\d{2})))?)?)?)?$");function o(t,e){var n=e>1?1:0;return r[e]+Math.floor((t-1969+n)/4)-Math.floor((t-1901+n)/100)+Math.floor((t-1601+n)/400)+365*(t-1970)}function i(e,r,n,o,c,a,l){var p,u=arguments.length;return this instanceof t?((p=1===u&&String(e)===e?new t(i.parse(e)):u>=7?new t(e,r,n,o,c,a,l):u>=6?new t(e,r,n,o,c,a):u>=5?new t(e,r,n,o,c):u>=4?new t(e,r,n,o):u>=3?new t(e,r,n):u>=2?new t(e,r):u>=1?new t(e):new t).constructor=i,p):t.apply(this,arguments)}for(e in t)i[e]=t[e];return i.now=t.now,i.UTC=t.UTC,i.prototype=t.prototype,i.prototype.constructor=i,i.parse=function(e){var r,i,c,a,l,p,u,f,s,h,y,g,b=n.exec(e);return b?(r=Number(b[1]),i=Number(b[2]||1)-1,c=Number(b[3]||1)-1,a=Number(b[4]||0),l=Number(b[5]||0),p=Number(b[6]||0),u=Math.floor(1e3*Number(b[7]||0)),f=!b[4]||b[8]?0:Number(new t(1970,0)),s="-"===b[9]?1:-1,h=Number(b[10]||0),y=Number(b[11]||0),a<(l>0||p>0||u>0?24:25)&&l<60&&p<60&&u<1e3&&i>-1&&i<12&&h<24&&y<60&&c>-1&&c<o(r,i+1)-o(r,i)&&-864e13<=(g=1e3*(60*((g=60*(24*(o(r,i)+c)+a+h*s))+l+y*s)+p)+u+f)&&g<=864e13?g:NaN):t.parse.apply(this,arguments)},i}(Date);try{-1===new Date(-621987552e5).toISOString().indexOf("-000001")&&delete Date.prototype.toISOString}catch(t){}Date.prototype.toISOString||(Date.prototype.toISOString=function(){var t,e,r,n;if(!isFinite(this))throw new RangeError("Date.prototype.toISOString called on non-finite value.");for(t=[this.getUTCMonth()+1,this.getUTCDate(),this.getUTCHours(),this.getUTCMinutes(),this.getUTCSeconds()],n=((n=this.getUTCFullYear())<0?"-":n>9999?"+":"")+("00000"+Math.abs(n)).slice(0<=n&&n<=9999?-4:-6),e=t.length;e--;)(r=t[e])<10&&(t[e]="0"+r);return n+"-"+t.slice(0,2).join("-")+"T"+t.slice(2).join(":")+"."+("000"+this.getUTCMilliseconds()).slice(-3)+"Z"});var S=!0;try{new Date(NaN).toJSON()}catch(t){S=!1}Date.prototype.toJSON&&S||(Date.prototype.toJSON=function(){if("function"!=typeof this.toISOString)throw new TypeError("toISOString property is not callable");try{return this.toISOString()}catch(t){return null}})}function E(t){var e=Number(t);return isNaN(e)?e=0:(0!==e||isFinite(e))&&(e=(e<0?-1:1)*Math.floor(Math.abs(e))),e}function m(t){if(null==t)throw new TypeError(t+" is not a object");return t&&y&&t instanceof String?t.split(""):Object(t)}function T(t,e){return e in t}function x(t){return Object.prototype.toString.call(t)}function P(t,e){if(null==t)throw new TypeError(e||"Cannot call method on "+t);return t}});
define("UWA/Internal/Immediate",[],function(){"use strict";var e,t,a,i=new Function("return this")();return i.setImmediate&&i.clearImmediate?e={set:i.setImmediate.bind(i),clear:i.clearImmediate.bind(i)}:i.addEventListener&&i.postMessage?(t={},a=0,i.addEventListener("message",function(e){var a;try{a="string"==typeof e.data&&"{"===e.data[0]&&JSON.parse(e.data)}catch(e){}a&&"uwa-setImmediate"===a.type&&e.source===i&&(e.stopPropagation(),t[a.id]&&(t[a.id](),delete t[a.id]))},!0),e={set:function(e){var n=a++;return t[n]=e,i.postMessage(JSON.stringify({type:"uwa-setImmediate",id:n}),"*"),n},clear:function(e){delete t[e]}}):e={set:function(e){return i.setTimeout(e,0)},clear:i.clearTimeout},e});
define("UWA/Internal/Polyfill/Promise",["UWA/Internal/Immediate"],function(e){"use strict";var r,t=new Function("return this")();t.UWA_SKIP_POLYFILLS||"function"!=typeof t.Promise&&((r=t.Promise=function(e){var r,t,n,i=this;if(!i||"object"!=typeof i)throw new TypeError("bad promise");if(void 0!==i._status)throw new TypeError("promise already initialized");if(!o(e))throw new TypeError("not a valid resolver");i._status="unresolved",i._resolveReactions=[],i._rejectReactions=[],r=function(e){"unresolved"===i._status&&(n=i._resolveReactions,i._result=e,u(i,n,"has-resolution"))},t=function(e){"unresolved"===i._status&&(n=i._rejectReactions,i._result=e,u(i,n,"has-rejection"))};try{e(r,t)}catch(e){t(e)}return i}).prototype={constructor:r,catch:function(e){return this.then(void 0,e)},then:function(e,t){var n,u,a,l;if(!function(e){return e instanceof r}(this))throw new TypeError("not a promise");switch(n=new i,o(t)||(t=function(e){throw e}),o(e)||(e=function(e){return e}),u=function(e,r,t){return function(n){if(n===e)return t(new TypeError("self resolution"));var o=new i;return s(n,o)?o.promise.then(r,t):r(n)}}(this,e,t),a={capability:n,handler:u},l={capability:n,handler:t},this._status){case"unresolved":this._resolveReactions.push(a),this._rejectReactions.push(l);break;case"has-resolution":c([a],this._result);break;case"has-rejection":c([l],this._result);break;default:throw new TypeError("unexpected")}return n.promise}},r.all=function(e){var t=new i,n=t.resolve,o=t.reject,s=[],c={count:1};try{a(e).forEach(function(e,n){var o,i,u=e._result,a=e._status;(o="has-resolution"===a?r.resolve(u):"has-rejection"===a?r.reject(u):e)&&(i=function(e,r,t,n){var o=!1;return function(i){o||(o=!0,r[e]=i,0==--n.count&&(0,t.resolve)(r))}}(n,s,t,c),c.count++,o.then(i,t.reject))}),0==--c.count&&n(s)}catch(e){o(e)}return t.promise},r.race=function(e){var r,t=new i,n=t.resolve,o=t.reject;try{a(e).forEach(function(e){var t,i=e._result,s=e._status;t="has-resolution"===s&&"has-rejection"!==r?n(i):"has-rejection"===s&&"has-resolution"!==r&&"has-rejection"!==r?o(i):e,r=s,t&&t.then(n,o)})}catch(e){o(e)}return t.promise},r.reject=function(e){var r=new i;return(0,r.reject)(e),r.promise},r.resolve=function(e){if(e instanceof r)return e;var t=new i;return(0,t.resolve)(e),t.promise});function n(e){return null!=e&&Object(e)===e}function o(e){return"function"==typeof e&&"[object Function]"===Object.prototype.toString.call(e)}function i(e){if(e){if(!o(e))throw new TypeError("bad promise constructor")}else e=r;var t,i=this;if(i.promise=Object.create(e.prototype||null),t=e.call(i.promise,function(e,r){i.resolve=e,i.reject=r}),!o(i.resolve)||!o(i.reject))throw new TypeError("bad promise constructor");if(n(t)&&t!==i.promise)throw new TypeError("bad promise constructor")}function s(e,r){if(!n(e))return!1;try{var t=e.then;if(!o(t))return!1;t.call(e,r.resolve,r.reject)}catch(e){r.reject(e)}return!0}function c(r,t){r.forEach(function(r){e.set(function(e,r){var t,n=r.handler,o=r.capability,i=o.resolve,c=o.reject;try{if((t=n(e))===o.promise)throw new TypeError("self resolution");s(t,o)||i(t)}catch(e){c(e)}}.bind(null,t,r))})}function u(r,t,n){e.clear(r._updateStatus),r._status=n,r._updateStatus=e.set(function(){r._resolveReactions=void 0,r._rejectReactions=void 0,c(t,r._result)})}function a(e){return function(e){if(Array.isArray(e))return e;if("number"!=typeof e.length)throw new TypeError("bad iterable");return Array.prototype.slice.call(e)}(e).map(function(e){return e instanceof r?e:r.resolve(e)})}});
define("UWA/Core",["UWA/Internal/Polyfill/NativeObjects","UWA/Internal/Polyfill/Promise"],function(){"use strict";var e,t,r,n,o=new Function("return this")(),a=Object.prototype.hasOwnProperty,i=Object.prototype.toString,l=o.UWA||{};return e={version:"1.3.RC4",hosts:function(){var e,t=o.document,r=t&&t.location&&"https:"===t.location.protocol?"https://":"http://",n=l.hosts,i={netvibes:"netvibes.com",uwa:"uwa.{netvibes}",exposition:"{uwa}",ecosystem:"eco.{netvibes}"};function c(e,t){return i[t].split("//")[1]}for(e in i)a.call(i,e)&&(n&&a.call(n,e)?i[e]=n[e]:i[e]=r+i[e].replace(/\{(\w+)\}/g,c));return i}(),paths:function(){var e,t=l.paths,r={lib:"/lib/",js:"/lib/UWA/js/",css:"/lib/c/UWA/assets/css/",img:"/lib/c/UWA/assets/img/"};for(e in r)a.call(r,e)&&t&&a.call(t,e)&&(r[e]=t[e]);return r}(),debug:Boolean(l.debug),namespace:function(t,r,n,a){n=n||o;var i,l,c=t.split("/");for(i=0,l=c.length;i<l;i++){t=c[i];var s=Boolean(n[t]);if(i===l-1){if(s){if(!a)throw new Error('Duplicate NameSpace "'+c.join(".")+'" into "'+n+'"');if("extend"===a)r=e.extend(n[t],r);else if("replace"===a)r=e.extend(r,n[t]);else{if(!0!==a)throw new Error("Unknown mode "+a);r=e.extend(n[t],r,!0)}}n[t]=r}else s||(n[t]={});n=n[t]}return r},getGlobal:function(){return o},extend:function(t,r,n){var o;for(o in r=r||{})if(a.call(r,o))if(n&&e.is(r[o],"plain"))e.is(t[o],"plain")||(t[o]={}),e.extend(t[o],r[o],n);else try{t[o]=r[o]}catch(e){}return t},merge:function(e,t){var r;for(r in t)a.call(t,r)&&(void 0!==e[r]&&null!==e[r]||(e[r]=t[r]));return e},clone:function(t,r){var n,o,i,l;switch(l=!0!==r&&!1!==r||r,e.typeOf(t)){case"array":if(l)for(n=[],o=0,i=t.length;o<i;o++)n[o]=e.clone(t[o],!0);else n=t.slice();break;case"object":if(l)for(o in n={},t)a.call(t,o)&&(n[o]=e.clone(t[o],!0));else n=e.extend({},t);break;case"date":n=new Date(t);break;case"element":n=t.cloneNode(l);break;default:n=t}return n},result:function(t,r,n){var o;return e.is(t)&&(o=t[r]),void 0===o&&(o=n),e.is(o,"function")?o.call(t):o},typeOf:(n={Null:!1,Undefined:!1,Function:"function",AsyncFunction:"function",String:"string",Array:"array",Date:"date",RegExp:"regexp",Number:"number",Boolean:"boolean",Error:"error",Arguments:"arguments",Blob:"blob",ArrayBuffer:"arraybuffer",FormData:"formdata",HTMLDocument:"document",XMLDocument:"document",Document:"document",global:"window",Window:"window",DOMWindow:"window",Math:"object",MouseEvent:"event",NodeList:"nodelist",Int8Array:"typedarray",Uint8Array:"typedarray",Uint8ClampedArray:"typedarray",Int16Array:"typedarray",Uint16Array:"typedarray",Int32Array:"typedarray",Uint32Array:"typedarray",Float32Array:"typedarray",Float64Array:"typedarray",DataView:"dataview",File:"file"},function(e){var t={}.toString.call(e).slice(8,-1);if(null==e)return!1;if("Function"===t&&"function"==typeof e.extend&&"function"==typeof e.singleton)return"class";if("Number"===t&&isNaN(e))return!1;if("Object"===t&&e&&"number"==typeof e.nodeType)return"element";var r=n[t];return void 0!==r?r:"Event"===t.slice(-5)?"event":"Element"===t.slice(-7)?"element":e.$extended&&e.event?"event":"Object"===t&&o.DataView&&e instanceof o.DataView?"dataview":"object"}),is:function(){var t;return t=Array.prototype.indexOf?function(e,t){return Array.prototype.indexOf.call(e,t)}:function(e,t){var r,n,o=!1;for(r=0,n=e.length;r<n;r++)if(e[r]===t){o=!0;break}return o?r:-1},function(r,n){var o,i;if(void 0===n)o="number"==typeof r?!isNaN(r):null!=r;else{if(n="array"===e.typeOf(n)?n:[n],o=!1,-1!==t(n,"finite")&&(o=isFinite(r)),o||-1===t(n,"plain")||(o=function(t){if(!t||"object"!==e.typeOf(t))return!1;try{if(t.constructor&&!a.call(t,"constructor")&&!a.call(t.constructor.prototype,"isPrototypeOf"))return!1}catch(e){return!1}var r;for(r in t)if(!a.call(t,r))return!1;return!0}(r)),!o){var l=t(n,"arraybufferview");l>=0&&(n=n.slice()).splice(l,1,"typedarray","dataview")}o||!1===(i=e.typeOf(r))||(o=-1!==t(n,i))}return o}}(),equals:function(){return function(t,r){return function t(r,n,o,a){var l,c,s,u,f,p,y;if(r===n)y=0!==r||1/r==1/n;else if(null==r||null==n)y=r===n;else if((l=i.call(r))!==i.call(n))y=!1;else if("[object String]"===l)y=String(r)===String(n);else if("[object Number]"===l)y=r!=Number(r)?n!=Number(n):0==r?1/r==1/n:r==Number(n);else if("[object Date]"===l||"[object Boolean]"===l)y=Number(r)===Number(n);else if("[object RegExp]"===l)y=r.source===n.source&&r.global===n.global&&r.multiline===n.multiline&&r.ignoreCase===n.ignoreCase;else if("object"!=typeof r||"object"!=typeof n)y=!1;else{for(c=o.length;c--;)o[c]===r&&(y=a[c]===n);if(void 0===y){if(o.push(r),a.push(n),"[object Array]"===l)for(y=(s=r.length)===n.length;y&&s>0;)y=t(r[--s],n[s],o,a);else if((u=r.constructor)===(f=n.constructor)||"[object Function]"===i.call(u)&&u instanceof u&&"[object Function]"===i.call(f)&&f instanceof f){for(p in s=0,y=!0,r)if(e.owns(r,p)&&(s++,!(y=e.owns(n,p)&&t(r[p],n[p],o,a))))break;if(y){for(p in n)if(e.owns(n,p)&&!s--)break;y=!s}}else y=!1;o.pop(),a.pop()}}return y}(t,r,[],[])}}(),owns:function(t,r){return e.is(t)&&a.call(t,r)},log:function(e,t){t||(t="log"),o.console?o.console[t](e):o.opera&&o.opera.postError&&o.opera.postError(e)},i18n:(r={},function(n,a){return a=a||(o.navigator?o.navigator.language||o.navigator.systemLanguage:"default"),t=r[a]=r[a]||{},"object"==typeof n?e.extend(t,n):t[n]||n}),driver:o.MooTools?"Mootools":"Alone"},define.amd&&define.amd.curl&&(o.require||o.curl)({apiName:"require",paths:{UWA:e.hosts.uwa+e.paths.js,vendors:e.hosts.uwa+e.paths.lib+"/vendors"}}),e.namespace("UWA",e,o,!0)});
define("UWA/Internal/Deprecate",["UWA/Core"],function(e){"use strict";var r={},t={warn:function(t,n,a){a||(a="warn"),e.debug&&!r.hasOwnProperty(t)&&(e.log(t+" is deprecated."+(n?" "+n:""),a),r[t]=!0)},alias:function(r,n,a){if(!e.debug)return a;var i=function(){return t.warn(r,n),a&&a.apply(this,arguments)};return a&&(i.prototype=a.prototype),i},property:function(r,n,a){var i=a?a.value:void 0;if(e.debug){var u=a&&a.name||n;Object.defineProperty(r,n,{get:function(){return t.warn(u,a&&a.message),i},set:function(e){t.warn(u,a&&a.message),i=e}})}else r[n]=i},uncurryAlias:function(e,r,n,a){Object.keys(e).forEach(function(i){var u=e[i];Object.defineProperty(r,i,{value:function(r,c,s){switch(t.warn(a+"#"+i,"Use "+n+"."+i+"(value, ...) instead"),arguments.length){case 0:return u.call(e,this);case 1:return u.call(e,this,r);case 2:return u.call(e,this,r,c);case 3:return u.call(e,this,r,c,s);default:var l=[].slice.call(arguments);return l.unshift(this),u.apply(e,l)}},writable:!0})})}};return t});
define("UWA/String",["UWA/Core","UWA/Internal/Deprecate"],function(UWA,Deprecate){"use strict";var Module={},isEmailRegExp,escapeSimpleComment,escapeMultiComment,alphaUpperRegExp,separatorDotRegExp,separatorRegExp,alphaRegExp,alphaUppperLowerRegExp,numRegExp;function parseColorToArray(e){var r,t,a=!1,n=(e=e.replace(/\s+/g,"")).match(/^rgb(a?)\(((?:\d{1,3},)*\d{1,3})\)/);if(n)a=n[2].split(",").map(function(e){return parseInt(e,10)}),(!n[1]&&3!==a.length||n[1]&&4!==a.length)&&(a=!1);else if(n=e.match(/^#?((?:[a-f0-9]{3}){1,2})$/i)){r=3===n[1].length?1:2,a=[];for(var i=0;i<n[1].length;i+=r)t=parseInt(n[1].substr(i,r),16),1===r&&(t=16*t+t),a.push(t)}else"transparent"===e&&(a=[0,0,0,0]);return a}function FakeString(){return Deprecate.warn("UWA/String as a constructor","Use the native String instead."),String.apply(null,arguments)}return Module.isEmail=(isEmailRegExp=/^([a-zA-Z0-9_.\-+])+@(([a-zA-Z0-9-])+\.)+([a-zA-Z0-9]{2,4})+$/,function(e){return isEmailRegExp.test(e)}),Module.truncate=function(e,r,t){return r=r||30,t=void 0===t?"...":t,e.length>r?e.slice(0,r-t.length)+t:String(e)},Module.cut=function(e,r,t){if(r=r||30,t=void 0===t?"...":t,e.length<=r)return String(e);var a,n=-1,i=t.length;for(a=r-i;a>=0;a--)if(-1!==".,;!? ".indexOf(e.charAt(a))){n=a;break}return n<0&&(n=r-i),e.slice(0,n)+t},Module.escapeRegExp=function(e){return e.replace(/\\/g,"\\\\").replace(/([-.*+?^$()[\]{}|])/g,"\\$1")},Module.stripTags=function(e){return e.replace(/ on\w+="[^"]*"/g,"").replace(/<(?!\s*\/?\s*(div|br|dt|dd|th|td|p|pre|h1|h2|h3|h4|h5)\b)[^>]*>/gi,"").replace(/<\/?[^>]+>/gi," ").replace(/^\s+|\s+$/g,"").replace(/\s+/g," ")},Module.stripScripts=function(string,evaluate){var scripts="",text=string.replace(/<script[^>]*>([\s\S]*?)<\/script>/gi,function(e,r){return scripts+=r+"\n",""});return!0===evaluate?eval(scripts):UWA.is(evaluate,"function")&&evaluate(scripts.trim(),text),text},Module.stripComments=(escapeSimpleComment=/^\/\/.*/gm,escapeMultiComment=/^\/\*[\S\s]*?\*\//gm,function(e){return e.replace(escapeSimpleComment,"").replace(escapeMultiComment,"")}),Module.escapeHTMLEntities=function(){var e={},r={apos:39,minus:8722,circ:710,tilde:732,Scaron:352,lsaquo:8249,OElig:338,lsquo:8216,rsquo:8217,ldquo:8220,rdquo:8221,bull:8226,ndash:8211,mdash:8212,trade:8482,scaron:353,rsaquo:8250,oelig:339,Yuml:376,yuml:255,fnof:402,Alpha:913,Beta:914,Gamma:915,Delta:916,Epsilon:917,Zeta:918,Eta:919,Theta:920,Iota:921,Kappa:922,Lambda:923,Mu:924,Nu:925,Xi:926,Omicron:927,Pi:928,Rho:929,Sigma:931,Tau:932,Upsilon:933,Phi:934,Chi:935,Psi:936,Omega:937,alpha:945,beta:946,gamma:947,delta:948,epsilon:949,zeta:950,eta:951,theta:952,iota:953,kappa:954,lambda:955,mu:956,nu:957,xi:958,omicron:959,pi:960,rho:961,sigmaf:962,sigma:963,tau:964,upsilon:965,phi:966,chi:967,psi:968,omega:969,thetasym:977,upsih:978,piv:982,ensp:8194,emsp:8195,thinsp:8201,zwnj:8204,zwj:8205,lrm:8206,rlm:8207,sbquo:8218,bdquo:8222,dagger:8224,Dagger:8225,hellip:8230,permil:8240,prime:8242,Prime:8243,oline:8254,frasl:8260,euro:8364,image:8465,weierp:8472,real:8476,alefsym:8501,larr:8592,uarr:8593,rarr:8594,darr:8595,harr:8596,crarr:8629,lArr:8656,uArr:8657,rArr:8658,dArr:8659,hArr:8660,forall:8704,part:8706,exist:8707,empty:8709,nabla:8711,isin:8712,notin:8713,ni:8715,prod:8719,sum:8721,lowast:8727,radic:8730,prop:8733,infin:8734,ang:8736,and:8743,or:8744,cap:8745,cup:8746,int:8747,there4:8756,sim:8764,cong:8773,asymp:8776,ne:8800,equiv:8801,le:8804,ge:8805,sub:8834,sup:8835,nsub:8836,sube:8838,supe:8839,oplus:8853,otimes:8855,perp:8869,sdot:8901,lceil:8968,rceil:8969,lfloor:8970,rfloor:8971,lang:9001,rang:9002,loz:9674,spades:9824,clubs:9827,hearts:9829,diams:9830,quot:34,amp:38,lt:60,gt:62,nbsp:160,iexcl:161,cent:162,pound:163,curren:164,yen:165,brvbar:166,sect:167,uml:168,copy:169,ordf:170,laquo:171,not:172,shy:173,reg:174,hibar:175,deg:176,plusmn:177,sup1:185,sup2:178,sup3:179,acute:180,micro:181,para:182,middot:183,cedil:184,ordm:186,raquo:187,frac14:188,frac12:189,frac34:190,iquest:191,Agrave:192,Aacute:193,Acirc:194,Atilde:195,Auml:196,Aring:197,AElig:198,Ccedil:199,Egrave:200,Eacute:201,Ecirc:202,Euml:203,Igrave:204,Iacute:205,Icirc:206,Iuml:207,ETH:208,Ntilde:209,Ograve:210,Oacute:211,Ocirc:212,Otilde:213,Ouml:214,times:215,Oslash:216,Ugrave:217,Uacute:218,Ucirc:219,Uuml:220,Yacute:221,THORN:222,szlig:223,agrave:224,aacute:225,acirc:226,atilde:227,auml:228,aring:229,aelig:230,ccedil:231,egrave:232,eacute:233,ecirc:234,euml:235,igrave:236,iacute:237,icirc:238,iuml:239,eth:240,ntilde:241,ograve:242,oacute:243,ocirc:244,otilde:245,ouml:246,divide:247,oslash:248,ugrave:249,uacute:250,ucirc:251,uuml:252,yacute:253,thorn:254};function t(r){return e[r]||(e[r]=new RegExp("&"+r+";","g")),e[r]}return function(e){var a,n;if(function(e){return e.match(/&([a-z]+;)/gi)}(e))for(a in r)r.hasOwnProperty(a)&&(n=t(a),e=e.replace(n,"&#"+r[a]+";"));return String(e)}}(),Module.globToRegex=function(e){var r=Module.escapeRegExp(e).replace(/\\\*/g,".*").replace(/\\\?/g,".").replace(/\\\{/g,"(").replace(/\\\}/g,")").replace(/,/g,"|");return new RegExp("^"+r+"$")},Module.escapeHTML=function(){var e={"&":"&amp;","<":"&lt;",">":"&gt;",'"':"&quot;","'":"&#x27;","/":"&#x2F;"},r=/[&<>"'/]/g,t=/[<>/]/g;function a(r){return e[r]}return function(e,n){return String(e).replace(n?t:r,a)}}(),Module.unescapeHTML=function(e){var r=document.createElement("div");return r.innerHTML=Module.stripTags(e).replace(/"/g,"&quot;"),r.childNodes[0]?r.childNodes[0].nodeValue:""},Module.ucfirst=function(e){return e.charAt(0).toUpperCase()+e.substr(1)},Module.lcfirst=function(e){return e.charAt(0).toLowerCase()+e.substr(1)},Module.capitalize=function(e){for(var r=e.toUpperCase(),t=e.toLowerCase(),a=!1,n="",i=0;i<e.length;i++)r[i]===t[i]?(n+=e[i],a=!1):a?n+=e[i]:(n+=r[i],a=!0);return n},Module.camelCase=(alphaUpperRegExp=/([A-Z]+)/g,separatorDotRegExp=/[-_\s](.)/g,separatorRegExp=/[-_\s]/g,function(e){return e=String(e).replace(alphaUpperRegExp,function(e,r){return r.substr(0,1).toUpperCase()+r.toLowerCase().substr(1,r.length)}).replace(separatorDotRegExp,function(e,r){return r.toUpperCase()}).replace(separatorRegExp,"").trim(),Module.lcfirst(e)}),Module.unCamelCase=(alphaRegExp=/([a-z])([A-Z])/g,alphaUppperLowerRegExp=/\b([A-Z]+)([A-Z])([a-z])/,function(e,r){return r=r||"-",e.toString().replace(alphaRegExp,"$1"+r+"$2").replace(alphaUppperLowerRegExp,"$1"+r+"$2$3").toLowerCase()}),Module.rgbToHex=function(e,r){var t=parseColorToArray(e);return t&&(t=r?t.map(function(e){return parseInt(e.toString(16),10)}):0===t[3]?"transparent":"#"+t.slice(0,3).map(function(e){return("0"+e.toString(16)).slice(-2)}).join("")),t},Module.hexToRgb=function(e,r){var t=parseColorToArray(e);return t&&!r&&(t=(3===t.length?"rgb(":"rgba(")+t.join(", ")+")"),t},Module.format=(numRegExp=/\{(\d+)\}/g,function(e){var r=arguments;return e.replace(numRegExp,function(e,t){return r[Number(t)+1]})}),Module.parseRelativeTime=function(e,r){var t,a,n,i,u=new Date,o=UWA.i18n;return u=new Date(u.getFullYear(),u.getMonth(),u.getDate()).getTime(),"number"!=typeof r&&(r=0),a=(t=e.match(/^(\d\d\d\d)-(\d\d)-(\d\d) (\d\d):(\d\d):(\d\d)$/))?new Date(t[1],t[2]-1,t[3],t[4],t[5],t[6]).getTime():/^\d{13}$/.test(e)?parseInt(e,10):/^\d{10}$/.test(e)?1e3*parseInt(e,10):Date.parse(e.replace(/\//g,"-")),r*=3600,n=(new Date-a)/1e3+r,i=(u-a)/1e3+r,!isNaN(n)&&(n<60?o("less than a minute ago"):n<120?o("about a minute ago"):n<2700?Module.format(o("{0} minutes ago"),Math.round(n/60)):n<5400?o("about an hour ago"):i<0?Module.format(o("about {0} hours ago"),Math.round(n/3600)):i<86400?o("yesterday"):Module.format(o("{0} days ago"),Math.ceil(i/86400)))},Module.makeClickable=function(e){var r=/((\w+:\/\/(\w+(:\w+)?@)?)|\bwww\.)[^\s<$]+/,t=/([/:\w+_-]+(\.[\w+_-]+)*@[\w.-]+)/;return e.replace(/(^|[\s>])([^\s<>"']+?)(?=$|[\s<])/gm,function(e,a,n){if(r.test(n)){var i=n.replace(/([.!?:)\]]$)/,""),u=n;return/^www\./.test(i)&&(i="http://"+i),a+'<a href="'+i+'" target="_blank">'+u+"</a>"}if(t.test(n)){var o=n;return/^[\w]+:\/\//.test(o)||(o='<a href="mailto:'+o+'">'+o+"</a>"),a+o}return e})},Module.contains=function(e,r,t){var a;return UWA.is(t,"string")?(e=t+e+t,r=t+r+t):UWA.is(t,"number")&&(a=t),-1!==e.indexOf(r,a)},Module.highlight=function(e){return Deprecate.warn("UWA.String.highlight"),e},Module.test=function(e,r,t){return Deprecate.warn("UWA.String.test","Use regexp.test(string) instead"),("string"==typeof r?new RegExp(r,t):r).test(e)},Deprecate.uncurryAlias(Module,String.prototype,"UWA.String","String"),Object.assign(FakeString,Module),UWA.namespace("String",FakeString,UWA)});
define("UWA/Array",["UWA/Core","UWA/Internal/Deprecate"],function(r,a){"use strict";var e={};function t(){return a.warn("UWA/Array as a constructor","Use the native Array instead."),Array.apply(null,arguments)}return e.equals=function(r,e){a.warn("UWA.Array.equals","Use UWA.equals instead");var t,n=r.length;if(!e||n!==e.length)return!1;for(t=0;t<n;t++)if(r[t]!==e[t])return!1;return!0},e.detect=function(r,a,e){var t,n;for(t=0,n=r.length;t<n;t++)if(a.call(e,r[t],t,r))return r[t]},e.invoke=function(r,a){var e=Array.prototype.slice.call(arguments,2);return r.map(function(r){return r[a].apply(r,e)})},e.erase=function(r,a){for(var e=r.length;e--;e)r[e]===a&&r.splice(e,1);return r},a.uncurryAlias(e,Array.prototype,"UWA.Array","Array"),t.isArray=a.alias("UWA/Array.isArray","Use the native Array.isArray instead",Array.isArray),["splice","slice"].forEach(function(r){t.prototype[r]=a.alias("UWA/Array#"+r,"Use the native Array#"+r+" instead",Array.prototype[r])}),Object.assign(t,e),r.namespace("Array",t,r)});
define("UWA/Utils",["UWA/Core","UWA/Array","UWA/Internal/Immediate"],function(e,t,r){"use strict";var n,o,a,i,c,l,s,u,D,B,p,A,f,C="ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789+/=",d=e.getGlobal();return n={buildUrl:function(){var e=d.location&&d.location.protocol?d.location.protocol:"http:";return function(t,r){if(t=String(t),r=String(r),!n.isAbsoluteUrl(t))throw new Error("First argument should be a absolute url.");"//"===t.substring(0,2)&&(t=e+t);var o,a,i,c,l=String(t).split("://"),s=l[0],u=l[1].split("/"),D=u[0],B="";if("//"===r.substring(0,2))t=s+":"+r;else if(r.split("://").length>1)t=r;else if("/"===r.substring(0,1))t=s+"://"+D+r;else{for(o=1,a=u.length-1;o<a;o++)B+="/"+u[o];t=s+"://"+D+(c=[],(i=B+"/"+r).replace(/^(\.\.?(\/|$))+/,"").replace(/\/(\.(\/|$))+/g,"/").replace(/\/\.\.$/,"/../").replace(/\/?[^/]*/g,function(e){"/.."===e?c.pop():c.push(e)}),c.join("").replace(/^\//,"/"===i.charAt(0)?"/":""))}return t}}(),parseUrl:(A=["source","subprotocol","protocol","authority","user","password","domain","port","path","directoryPath","fileName","query","anchor"],f=new RegExp("^(?:(?:(?:([^#.:]+):)?([^#.:]+):)?//)?((?:([^:/]+)(?::([^/]*?))?@)?([^:/?#]*)(?::(\\d*))?)?((/(?:[^?#](?![^?#/]*\\.[^?#/.]+(?:[\\?#]|$)))*/?)?([^?#/]*))?(?:\\?([^#]*))?(?:#(.*))?"),function(e){var t,r=f.exec(e),n={};for(t=0;t<A.length;t++)n[A[t]]=r[t]||"";return n.subprotocol&&(n.source=n.source.substr(n.subprotocol.length+1)),n.port||(n.port="https"===n.protocol?"443":"80"),n.directoryPath&&n.directoryPath.length>0&&(n.directoryPath=n.directoryPath.replace(/\/?$/,"/")),n.domain=n.domain.toLocaleLowerCase(),n.protocol=n.protocol.toLocaleLowerCase(),n}),composeUrl:function(e){var t="";return e.protocol&&(t=e.protocol+"://",e.subprotocol&&(t=e.subprotocol+":"+t)),e.domain?(t+=e.domain,!e.port||"http"===e.protocol&&80===parseInt(e.port,10)||"https"===e.protocol&&443===parseInt(e.port,10)||(t+=":"+e.port)):e.authority&&(t+=e.authority),e.path&&(t+=e.path),e.query&&(t+="?"+e.query),e.anchor&&(t+="#"+e.anchor),t},matchUrl:function(e,t){var r,o,a=!1,i=n.isAbsoluteUrl(e),c=n.isAbsoluteUrl(t);return i||c?(i?c||(t=n.buildUrl(e,t)):e=n.buildUrl(t,e),r=n.parseUrl(e),o=n.parseUrl(t),a=["domain","protocol","port"].every(function(e){return r[e]===o[e]||"protocol"===e&&(""===r[e]||""===o[e])})):a=!0,a},isAbsoluteUrl:(p=/^((https?|ftp|file):)?\/\//i,function(e){return p.test(e)}),isValidUrl:(u="(\\/(?!/)([a-z0-9._~\\u00A0-\\uD7FF\\uF900-\\uFDCF\\uFDF0-\\uFFEF!\\$&'\\(\\)\\*\\+,;=:@-]|(?:%[\\da-f]{2}))*)*(\\?(([a-z0-9._~\\u00A0-\\uD7FF\\uF900-\\uFDCF\\uFDF0-\\uFFEF!\\$&'\\(\\)\\*\\+,;=:@-]|(?:%[\\da-f]{2}))|[\\uE000-\\uF8FF]|\\/|\\?)*)?(\\#(([a-z0-9._~\\u00A0-\\uD7FF\\uF900-\\uFDCF\\uFDF0-\\uFFEF!\\$&'\\(\\)\\*\\+,;=:@-]|(?:%[\\da-f]{2}))|[\\uE000-\\uF8FF]|\\/|\\?)*)?",D=new RegExp("^(?:((?:https?|ftp|file):)?//)(?:\\S+(?::\\S*)?@)?(?:(?:[1-9]\\d?|1\\d\\d|2[01]\\d|22[0-3])(?:\\.(?:1?\\d{1,2}|2[0-4]\\d|25[0-5])){2}(?:\\.(?:[1-9]\\d?|1\\d\\d|2[0-4]\\d|25[0-4]))|(?:[a-z\\u00a1-\\uffff0-9]+-)*[a-z\\u00a1-\\uffff0-9]+(?:\\.(?:[a-z\\u00a1-\\uffff0-9]+-)*[a-z\\u00a1-\\uffff0-9]+)*\\.(?:[a-z\\u00a1-\\uffff]{2,}))(?::\\d{2,5})?"+u+"$","i"),B=new RegExp("^"+u+"$","i"),function(e){return(n.isAbsoluteUrl(e)?D:B).test(e)}),encodeUrl:function(e){return encodeURIComponent(e).replace(/\./g,"%2e")},parseQuery:function(t){var r=t.substring(t.indexOf("?")+1).split(/[&;]/),n={};return r.length&&r.forEach(function(t){var r=t.indexOf("=")+1,o=r?t.substr(r):"",a=r?t.substr(0,r-1).match(/([^\][]+|(\B)(?=\]))/g):[t],i=n;a&&(o=decodeURIComponent(o),a.forEach(function(t,r){t=decodeURIComponent(t);var n=i[t];r<a.length-1?i=i[t]=n||{}:Array.isArray(n)?n.push(o):i[t]=e.is(n)?[n,o]:o}))}),n},toQueryString:function(t,r){var o,a,i,c,l=e.is;if(l(t,"string"))c=t;else if(l(t.toQueryString,"function"))c=t.toQueryString();else{for(o in c=[],t)t.hasOwnProperty(o)&&(a=t[o],r&&(o=r+"["+o+"]"),l(a)&&(l(a,"object")||l(a,"array")?i=n.toQueryString(a,o):l(a,"function")||(i=n.encodeUrl(o)+"="+n.encodeUrl(a))),i&&c.push(i),i=void 0);c=c.join("&")}return c},getQueryString:function(e,t,r){t=t.replace(/[[]/,"\\[").replace(/[\]]/,"\\]");var n=new RegExp(t+"=([^&#]*)").exec(e);return n?decodeURIComponent(n[1]):r},loadXml:(c=/<(DOCTYPE|xml)[^><]*>|<.(DOCTYPE|xml)[^><]*>/g,l=/(<(style|script)[^>]*>)([\u0001-\uFFFF]*?)(<\/(style|script)>)/gim,s=/<!\[CDATA\[/,function(e,t){var r,o,a,i,u;if("object"==typeof e&&e.nodeType)r=e;else if(e=(e=e.replace(c,"")).replace(l,function(){var e=arguments,t=e[1],r=e[3],n=e[4];return s.test(r)||(r="<![CDATA[\n"+r+"\n]]>"),t+r+n}),d.DOMParser)try{if(u=(r=(r=new d.DOMParser).parseFromString(e,"application/xml")).getElementsByTagName("parsererror")[0])throw new Error(u.textContent||u.innerText)}catch(e){throw new Error("Invalid XML: "+e.message)}else{if(!d.ActiveXObject)throw new Error("No native XML parser available.");if((r=new d.ActiveXObject("MSXML2.DOMDocument")).setProperty("SelectionLanguage","XPath"),r.validateOnParse=!1,r.resolveExternals=!1,r.preserveWhiteSpace=!1,r.async=!1,r.loadXML(e),0!==r.parseError.errorCode)throw new Error("Invalid XML: "+r.parseError.line+", "+r.parseError.reason)}return t&&(d.XSLTProcessor?((o=new d.XSLTProcessor).importStylesheet(n.loadXml(t)),r=o.transformToDocument(r,document)):((o=new d.ActiveXObject("Msxml2.FreeThreadedDOMDocument")).loadXML(n.xmlToString(t)),(a=new d.ActiveXObject("Msxml2.XSLTemplate")).stylesheet=o,(i=a.createProcessor()).input=r,i.transform(),r=n.loadXml(i.output))),r}),loadHtml:function(){var e=new RegExp("</?(script|embed|object|frameset|frame|iframe|meta|link|style)(.|\n)*?>","img"),t=new RegExp("<([a-z][a-z0-9]*)(?:[^>]*(\\s(src|href|title|style|alt|height|width|data-([a-z][a-z0-9]*))=['\"][^'\"]*['\"]))?[^>]*?(\\/?)>","im");return function(r){var n,o,a,i;if(d.DOMParser)try{n=(new d.DOMParser).parseFromString(r,"text/html")}catch(e){}if(!n&&document.implementation.createHTMLDocument)try{(o=(n=document.implementation.createHTMLDocument("")).documentElement).innerHTML=r,a=o.firstElementChild,1===o.childElementCount&&"html"===a.localName.toLowerCase()&&n.replaceChild(a,o)}catch(e){n=null}if(r=function(r){return r=(r=r.replace(e,"")).replace(t,"<$1$2$4>")}(r),!n&&d.ActiveXObject)try{(n=new d.ActiveXObject("htmlfile")).write(r),n.close()}catch(e){n=null}return n||((i=document.createElement("iframe")).style.display="none",document.body.appendChild(i),(n=i.contentDocument||i.contentWindow.document).write(r),n.close(),document.body.removeChild(i)),n}}(),xmlToHtml:function(e){"string"==typeof e&&(e=n.loadXml(e)),9===e.nodeType&&(e=e.childNodes[0]);var t,r,o,a,i=e.nodeName.toLowerCase(),c=document.createElement(i),l=e.childNodes,s=e.attributes||[];for(o=0,a=s.length;o<a;o++)t=s[o],c.setAttribute(t.name,t.value);for(o=0,a=l.length;o<a;o++)switch((r=l[o]).nodeType){case 1:c.appendChild(n.xmlToHtml(r));break;case 3:"style"===i&&c.styleSheet?c.styleSheet.cssText=r.nodeValue:c.appendChild(document.createTextNode(r.nodeValue));break;case 4:case 8:"script"===i?c.text=r.nodeValue:c.appendChild(document.createComment(r.nodeValue))}return c},xmlToString:function(){return function(e,t){var r;return r="string"==typeof e?e:d.XMLSerializer?(r=new d.XMLSerializer).serializeToString(e):e.xml,t&&(r=function(e){var t,r,n,o,a=0;return t=e.trim().replace(/(>)(\s+)?(<)(\/*)/g,"$1\r\n$3$4").split(">\r\n"),e="",t.forEach(function(i,c){var l,s=0,u="",D="\r\n";for(c!==t.length-1&&(i+=">"),n=o,o=r,r=/(<!\[CDATA\[)|(\]\]>)/.test(t[c+1]||""),i.match(/.+<\/\w[^>]*>$/)?s=0:i.match(/^<\/\w/)?0!==a&&(a-=1):i.match(/^<\w[^>]*[^/]>.*$/)&&(s=1),l=0;l<a;l++)u+="  ";(r||o&&!r)&&(D=""),(o||n&&!o)&&(u=""),e+=u+i+D,a+=s}),e}(r)),r.trim()}}(),setCss:function(){function e(e,t){var r,n,o=t.match(/^[\s\S]*(?:^|\s)(?:body|html)\b(\S*)/);return o?(r=t.slice(0,o[0].length).trim()+" ",n=t.slice(o[0].length).trim()):(r="",n=t),(n=n.replace(/^\.module\b\S*\s/,"")).startsWith(e+" ")||(n=e+" "+n),r+n}return function(r,o,a,i){a=a?a.trim():"",o=Array.isArray(o)?o.join("\n"):String(o),r||(r=n.getCheckSum(o));var c=function(e){for(var t=/\{/g,r=/\}/g,n=0,o=r.test(e),a=t.test(e),i=[],c={children:i};;)if(a&&t.lastIndex<r.lastIndex){var l={prefix:e.slice(n,t.lastIndex-1),parent:c,content:"",children:[]};c.children.push(l),c=l,n=t.lastIndex,a=t.test(e)}else{if(!o)break;c.content=e.slice(n,r.lastIndex-1),c.parent&&(c=c.parent),n=r.lastIndex,o=r.test(e)}return i}(o=o.replace(/\/\*[\s\S]*?\*\//g,""));return a&&(!function e(r,n){r.forEach(function(r){var o=r.prefix.trim();"@"!==o[0]&&!1!==n&&(r.selectors=t.invoke(o.split(","),"trim")),e(r.children,!o.startsWith("@keyframes"))})}(c),function t(r,n){r.forEach(function(r){var o,a;if(r.selectors)for(o=0,a=r.selectors.length;o<a;o++)r.selectors[o]=e(n,r.selectors[o]);else t(r.children,n)})}(c,a)),i&&function(e,t){e.forEach(function(e){e.content=e.content.replace(/\burl\(["']?([\s\S]*?)["']?\)/g,function(e,r){return n.isAbsoluteUrl(r)||(r=n.buildUrl(t,r)),'url("'+r+'")'})})}(c,i),function(e,t){var r=document.getElementById(t);r||((r=document.createElement("style")).setAttribute("id",t),r.setAttribute("type","text/css"),document.getElementsByTagName("head").item(0).appendChild(r)),r.styleSheet?r.styleSheet.cssText=e:r.appendChild(document.createTextNode(e))}(o=function e(t){return t.map(function(t){return(t.selectors?t.selectors.join(",\n")+" ":t.prefix)+"{"+e(t.children)+t.content+"}"}).join("\n")}(c),r),o}}(),toArray:function(e){var t,r,n=typeof e,o=[];if("string"===n)o=e.split("");else if("object"===n&&!1===Array.isArray(e))if(void 0!==e.length)for(t=0,r=e.length;t<r;t++)o[t]=e[t];else for(t in e)e.hasOwnProperty(t)&&o.push(e[t]);else e&&(o=Array.prototype.slice.call(e));return o},splat:function(t){return e.is(t)?Array.isArray(t)?t:e.is(t,"arguments")?n.toArray(t):[t]:[]},getUUID:function(){return"xxxxxxxx-xxxx-4xxx-yxxx-xxxxxxxxxxxx".replace(/[xy]/g,function(e){var t=16*Math.random()|0;return("x"===e?t:3&t|8).toString(16)})},getUniqueId:(a=0,i=Math.pow(32,4),function(e){return a++,(e||"u")+("0000"+((Math.random()*i|0)*i+a).toString(32)).slice(-8)}),getCheckSum:function(e,t){var r,n;for(t=t||305419896,r=0,n=(e=String(e)).length;r<n;r++)t+=e.charCodeAt(r)*r;return Math.abs(parseInt(t,10)).toString(36)},getCRC32:(o="00000000 77073096 EE0E612C 990951BA 076DC419 706AF48F E963A535 9E6495A3 0EDB8832 79DCB8A4 E0D5E91E 97D2D988 09B64C2B 7EB17CBD E7B82D07 90BF1D91 1DB71064 6AB020F2 F3B97148 84BE41DE 1ADAD47D 6DDDE4EB F4D4B551 83D385C7 136C9856 646BA8C0 FD62F97A 8A65C9EC 14015C4F 63066CD9 FA0F3D63 8D080DF5 3B6E20C8 4C69105E D56041E4 A2677172 3C03E4D1 4B04D447 D20D85FD A50AB56B 35B5A8FA 42B2986C DBBBC9D6 ACBCF940 32D86CE3 45DF5C75 DCD60DCF ABD13D59 26D930AC 51DE003A C8D75180 BFD06116 21B4F4B5 56B3C423 CFBA9599 B8BDA50F 2802B89E 5F058808 C60CD9B2 B10BE924 2F6F7C87 58684C11 C1611DAB B6662D3D 76DC4190 01DB7106 98D220BC EFD5102A 71B18589 06B6B51F 9FBFE4A5 E8B8D433 7807C9A2 0F00F934 9609A88E E10E9818 7F6A0DBB 086D3D2D 91646C97 E6635C01 6B6B51F4 1C6C6162 856530D8 F262004E 6C0695ED 1B01A57B 8208F4C1 F50FC457 65B0D9C6 12B7E950 8BBEB8EA FCB9887C 62DD1DDF 15DA2D49 8CD37CF3 FBD44C65 4DB26158 3AB551CE A3BC0074 D4BB30E2 4ADFA541 3DD895D7 A4D1C46D D3D6F4FB 4369E96A 346ED9FC AD678846 DA60B8D0 44042D73 33031DE5 AA0A4C5F DD0D7CC9 5005713C 270241AA BE0B1010 C90C2086 5768B525 206F85B3 B966D409 CE61E49F 5EDEF90E 29D9C998 B0D09822 C7D7A8B4 59B33D17 2EB40D81 B7BD5C3B C0BA6CAD EDB88320 9ABFB3B6 03B6E20C 74B1D29A EAD54739 9DD277AF 04DB2615 73DC1683 E3630B12 94643B84 0D6D6A3E 7A6A5AA8 E40ECF0B 9309FF9D 0A00AE27 7D079EB1 F00F9344 8708A3D2 1E01F268 6906C2FE F762575D 806567CB 196C3671 6E6B06E7 FED41B76 89D32BE0 10DA7A5A 67DD4ACC F9B9DF6F 8EBEEFF9 17B7BE43 60B08ED5 D6D6A3E8 A1D1937E 38D8C2C4 4FDFF252 D1BB67F1 A6BC5767 3FB506DD 48B2364B D80D2BDA AF0A1B4C 36034AF6 41047A60 DF60EFC3 A867DF55 316E8EEF 4669BE79 CB61B38C BC66831A 256FD2A0 5268E236 CC0C7795 BB0B4703 220216B9 5505262F C5BA3BBE B2BD0B28 2BB45A92 5CB36A04 C2D7FFA7 B5D0CF31 2CD99E8B 5BDEAE1D 9B64C2B0 EC63F226 756AA39C 026D930A 9C0906A9 EB0E363F 72076785 05005713 95BF4A82 E2B87A14 7BB12BAE 0CB61B38 92D28E9B E5D5BE0D 7CDCEFB7 0BDBDF21 86D3D2D4 F1D4E242 68DDB3F8 1FDA836E 81BE16CD F6B9265B 6FB077E1 18B74777 88085AE6 FF0F6A70 66063BCA 11010B5C 8F659EFF F862AE69 616BFFD3 166CCF45 A00AE278 D70DD2EE 4E048354 3903B3C2 A7672661 D06016F7 4969474D 3E6E77DB AED16A4A D9D65ADC 40DF0B66 37D83BF0 A9BCAE53 DEBB9EC5 47B2CF7F 30B5FFE9 BDBDF21C CABAC28A 53B39330 24B4A3A6 BAD03605 CDD70693 54DE5729 23D967BF B3667A2E C4614AB8 5D681B02 2A6F2B94 B40BBE37 C30C8EA1 5A05DF1B 2D02EF8D",function(e){var t,r,n=0,a=0;for(n^=-1,t=0,r=(e=String(e)).length;t<r;t++)a=255&(n^e.charCodeAt(t)),n=n>>>8^"0x"+o.substr(9*a,8);return-1^n}),base64Encode:function(){var e=d.btoa||function(e){for(var t,r,n,o,a,i,c,l=e.length,s="",u=0;u<l;)o=(t=e.charCodeAt(u++))>>2,a=(3&t)<<4|(r=e.charCodeAt(u++))>>4,i=(15&r)<<2|(n=e.charCodeAt(u++))>>6,c=63&n,isNaN(r)?i=c=64:isNaN(n)&&(c=64),s=s+C.charAt(o)+C.charAt(a)+C.charAt(i)+C.charAt(c);return s};return function(t){return t=String(t),e(unescape(encodeURIComponent(t)))}}(),base64Decode:function(){var e=/[^A-Za-z0-9+/=]/g,t=d.atob||function(t){var r,n,o,a,i,c,l,s,u="",D=0;if("string"!=typeof t&&(t=String(t)),(r=(t=t.replace(e,"")).length)%4==1)throw new Error("InvalidCharacterError: DOM Exception 5");for(;D<r;)i=C.indexOf(t.charAt(D++)),c=C.indexOf(t.charAt(D++)),l=D<r&&C.indexOf(t.charAt(D++)),s=D<r&&C.indexOf(t.charAt(D++)),n=i<<2|c>>4,u+=String.fromCharCode(n),!1!==l&&64!==l&&(o=(15&c)<<4|l>>2,u+=String.fromCharCode(o)),!1!==s&&64!==s&&(a=(3&l)<<6|s,u+=String.fromCharCode(a));return u};return function(e){var r=t(e);try{r=decodeURIComponent(escape(r))}catch(e){}return r}}(),attempt:function(t,r,n){var o,a=Array.prototype.slice.call(arguments,3);if(e.debug)o=t.apply(n,a);else try{o=t.apply(n,a)}catch(t){r?o=r.apply(n,[t].concat(a)):e.log("Error in Utils.attempt: "+t)}return o},memoize:function(e,t){var r={},n=Array.prototype.slice;return t=t||JSON.stringify,function(){var o=t(n.call(arguments));return r.hasOwnProperty(o)||(r[o]=e.apply(this,arguments)),r[o]}},getOwnPropertyMatchName:function(e,t){var r,n;if(t=String(t),e.hasOwnProperty(t))n=t;else for(r in t=t.toLowerCase(),e)if(e.hasOwnProperty(r)&&r.toLowerCase()===t){n=r;break}return n},getOwnPropertyMatchValue:function(e,t){var r=n.getOwnPropertyMatchName(e,t);return r?e[r]:void 0},setImmediate:r.set,clearImmediate:r.clear,random:function(t,r){return e.is(r)||(r=t,t=0),t+Math.floor(Math.random()*(r-t+1))}},e.namespace("Utils",n,e,!0)});
define("UWA/Utils/Client",["UWA/Core","UWA/Utils"],function(e,n){"use strict";var t,o,i,a,r,d,s=e.getGlobal(),l=Boolean(s.window),c=Boolean(l&&window.document),m=Boolean(l&&window.navigator),u=Boolean(l&&window.matchMedia),w=(o=["","moz","Moz","MOZ","webkit","Webkit","WebKit","WEBKIT","ms","Ms","MS","o","O"],function(e,n,t){var i,a,r,d,s,l,c=n.indexOf("{}");for(c>=0?(a=n.slice(0,c),r=n.slice(c+2)):(a="",r=n),i=r.charAt(0).toUpperCase()+r.slice(1),d=0,s=o.length;d<s&&!((l=a+o[d]+r)in e)&&!((l=a+o[d]+i)in e);d++);if(d<s)return t?l:e[l]});return(t={Engine:{name:"unknown",version:0},Platform:{name:"unknown"},Features:{window:l,document:c,navigator:m,xpath:c&&Boolean(document.evaluate),json:l&&Boolean(window.JSON),orientation:l&&Boolean(window.orientation),querySelector:c&&Boolean(document.querySelector),fullscreen:Boolean(w(document,"exitFullscreen")||w(document,"cancelFullScreen")),inputPlaceholder:void 0!==document.createElement("input").placeholder,cors:l&&"withCredentials"in new window.XMLHttpRequest,touchEvents:l&&Boolean("ontouchstart"in window||window.DocumentTouch&&document instanceof window.DocumentTouch),pointerEvents:m&&Boolean(navigator.msPointerEnable||navigator.pointerEnabled),mutationEvents:Boolean(c&&document.implementation&&document.implementation.hasFeature("MutationEvents","2.0"))||l&&window.MutationEvent,eventCapture:l&&Boolean(window.addEventListener),flexboxCSS:c&&Boolean(w(document.createElement("div").style,"flexBasis",!0)),filterCSS:c&&!(document.documentElement&&document.documentElement.style.filter),opacityCSS:c&&!(document.documentElement&&document.documentElement.style.opacity),transitionsCSS:c&&Boolean(w(document.createElement("div").style,"transition",!0)),stickyCSS:c&&(d=document.createElement("div").style,d.position="-webkit-sticky",d.position="sticky",Boolean(d.position)),matrixCSS:(r=l&&w(window,"CSSMatrix"),Boolean(r)&&void 0!==(new r).m11),dragAndDrop:l&&!(window.System&&window.System.Gadget),mediaQueryList:u,touch:l&&m&&function(){var e=!1;if("maxTouchPoints"in navigator)e=navigator.maxTouchPoints>0;else if("msMaxTouchPoints"in navigator)e=navigator.msMaxTouchPoints>0;else{var n=window.matchMedia&&matchMedia("(pointer:coarse)");if(n&&"(pointer:coarse)"===n.media)e=Boolean(n.matches);else if("orientation"in window)e=!0;else{var t=navigator.userAgent;e=/\b(BlackBerry|webOS|iPhone|IEMobile)\b/i.test(t)||/\b(Android|Windows Phone|iPad|iPod)\b/i.test(t)}}return Boolean(e)}()},Locale:(i=(m&&(navigator.languages&&navigator.languages[0]||navigator.language||navigator.userLanguage)||"en-US").toLowerCase().split("-"),a=i[0]||"en",{lang:a,locale:i[1]||"us",dir:-1!==["ar","he"].indexOf(a)?"rtl":"ltr"}),detect:function(){var e=/(opera|ie|firefox|chrome|version)[\s/:]([\w\d.]+)[\s/:](safari|version)[\s/:]([\w\d.]+)[\s/:](vivaldi|opr|mms|edg)[\s/:]([\w\d.]+)/,n=/(opera|ie|firefox|chrome|version)[\s/:]([\w\d.]+)?.*?(safari|version[\s/:]([\w\d.]+)|$)/,o=/(webkit)\s\/:(\w\d\.+)/,i=/(trident)\/.*rv:([\d.]+)/,a=/ip(?:ad|od|hone)/,r=/webos|wossystem/,d=/blackberry/,l=/android/,u=/\bphantomjs\b/i,w=/mac|win|linux/;function h(){return m&&navigator.userAgent.toLowerCase()||""}return function(){var p,v,g,f,b,E;t.Engine=(E=h(),f="ie"===(v=E.match(e)||E.match(n)||E.match(o)||E.match(i)||(s.process?[null,"nodeJS",s.process.version]:[null,"unknown",0]))[1]&&c&&document.documentMode||("opera"===v[1]&&v[4]?v[4]:v[2]),b=parseInt(f,10),v[5]&&v[6]?(g=v[5],f=v[6],b=parseInt(f,10)):g="version"===v[1]?v[3]:v[1],"trident"===g?g="ie":"opr"===g?g="opera":"mms"===g?g="opera-neon":"edg"===g&&(g="edge"),(p={name:g,version:b,fullVersion:f})[g]=b,p[g+b]=!0,p.webkit=Boolean(E.match(/webkit/)),p),t.Platform=function(){var e,n=function(){var e=(m&&navigator.platform.toLowerCase()||"").split(" ")[0],n=h(),t=new RegExp("win64","gi"),o=new RegExp("x64","gi"),i=new RegExp("wow64","gi");return e.match(/win32/i)&&(t.test(n)||o.test(n)||i.test(n))&&(e="win64"),e}(),o=h();(e={name:a.test(o)?"ios":r.test(o)?"webos":d.test(o)?"blackberry":l.test(o)?"android":u.test(o)?"phantomjs":w.test(n)||s.process?n:"other"})[e.name]=!0;var i=o.match(/ipad/)||"MacIntel"===navigator.platform&&navigator.maxTouchPoints>1;return e.ipad=Boolean(i),e.tablet=e.ipad||Boolean(o.match(/tablet/))||Boolean(o.match(/sm-t\d+/i)),e.windows=0===e.name.indexOf("win"),"macintel"===e.name&&i&&t.Features.touch&&(e.name="ios",e.macintel=!1,e.ios=!0),e}(),c&&(document.documentElement.className+=" "+t.Engine.name+" "+t.Engine.name+t.Engine.version+" "+t.Platform.name)}}(),isOnline:function(e,n){return void 0!==e&&n?(t.onLine=Boolean(e),setTimeout(function(){delete t.onLine},n)):void 0===t.onLine&&(t.Platform.phantomjs||!m||void 0===navigator.onLine?t.onLine=!0:t.onLine=!0===navigator.onLine),t.onLine},getOrientation:l&&window.self===window.top&&window.orientation?function(){var e=window.orientation;return 90===Math.abs(e)?"landscape":"portrait"}:function(){var e=t.getSize();return e.width/e.height<1?"portrait":"landscape"},getSize:function(){var e,n,t=0,o=0;return l&&"number"==typeof window.innerWidth?(t=window.innerWidth,o=window.innerHeight):c&&(e=document.documentElement,n=document.body,e&&(e.clientWidth||e.clientHeight)?(t=e.clientWidth,o=e.clientHeight):n&&(n.clientWidth||n.clientHeight)&&(t=n.clientWidth,o=n.clientHeight)),{width:t,height:o}},getScrolls:function(){var e=0,n=0;return l&&"number"==typeof window.pageYOffset&&(n=window.pageYOffset,e=window.pageXOffset),{y:n,x:e}},getScrollbarWidth:n.memoize(function(){var e,n,t=0;return c&&(e=document.documentElement,(n=document.createElement("div")).style.cssText="width:100px;height:100px;overflow:scroll;position:absolute;top:-9999px;",e.appendChild(n),t=n.offsetWidth-n.clientWidth,e.removeChild(n)),t}),addStar:function(e,n){if(l)if(window.sidebar)window.sidebar.addPanel(n,e,"");else if(window.external)window.external.AddFavorite(e,n);else if(window.opera&&window.print)return!0},getVendorProperty:w}).detect(),e.namespace("Utils/Client",t,e)});
define("UWA/Class",["UWA/Core"],function(t){"use strict";var n=!1,i=/xyz/.test(function(){t.xyz()}),e=i?/\b_parent\b/:/^/,r=i?/\b_previous\b/:/^/,o=function(){},s=function(){};function a(t,n,i,s){i._original&&(i=i._original);var a,p=e.test(i),u=r.test(i);return p||u?("function"!=typeof n&&(n=s?o:t||o),"function"!=typeof t&&(t=u?o:n),(a=function(){var e,r,o;return null!=this?(p&&(r=this._parent,this._parent=t),u&&(o=this._previous,this._previous=n),e=i.apply(this,arguments),p&&(this._parent=r),u&&(this._previous=o)):e=i.apply(this,arguments),e}).displayName="(method wrapper)",a._original=i,a):i}function p(t){return function(){this._previous.apply(this,arguments),t.apply(this,arguments)}}return s.extend=function(){var i,e;return n=!0,i=new this,n=!1,e=function(){!n&&this.__uwaPrivateConstructor&&this.__uwaPrivateConstructor.apply(this,arguments)},i.constructor=e,t.extend(e,{prototype:i,parent:this,extend:s.extend,singleton:s.singleton,implement:s.implement}),e.implement.apply(e,arguments),e},s.implement=function(){var n,i,e,r,o,s,u,l=this.prototype||this;for(n=0,i=arguments.length;n<i;n+=1){var c;for(r in e=arguments[n],"class"===(o=t.typeOf(e))||"function"===o?("function"===o&&(e.prototype.__uwaPrivateConstructor=p(e)),e=e.prototype):e.init&&(e.__uwaPrivateConstructor=e.init,delete e.init),c=e.name?e.name:l.name?t.owns(l,"name")?l.name:"("+l.name+" inheritor)":"(anonymous class)",e)"constructor"!==r&&(s=e[r],t.is(s,"function")?(u=("class"===o?arguments[n]:this).parent,s.displayName=c+"#"+("__uwaPrivateConstructor"===r?"init":r),l[r]=a(u&&u.prototype&&u.prototype[r],t.owns(l,r)&&l[r],s,"class"===o)):t.is(s,"plain")?(t.owns(l,r)||(l[r]=t.is(l[r],"plain")?t.clone(l[r]):{}),t.extend(l[r],s,!0)):l[r]=s)}return this},s.singleton=function(){var t,i=this.extend.apply(this,arguments),e=i.prototype,r=!1,o=[];function s(n){t[n]=function(){if(!r){if("throw"===t.uninitializedCalls)throw new Error("Singleton called before being initialized");if("ignore"===t.uninitializedCalls)return;t.init()}return t[n].apply(this,arguments)}}for(var a in n=!0,t=new i,n=!1,e)"function"==typeof e[a]&&"init"!==a&&"constructor"!==a&&(o.push(a),s(a));return t.init=function(){if(r)throw new Error("Singleton is already initialized");var n,e;for(r=!0,n=0,e=o.length;n<e;n++)delete t[o[n]];return i.apply(this,arguments),this},t},t.namespace("Class",s,t)});
define("UWA/Dispatcher",["UWA/Core","UWA/Utils","UWA/Class"],function(i,t,e){"use strict";var n=i.Class.extend({Binding:null,bindings:null,shouldPropagate:!0,active:!0,dispatching:0,init:function(){this.bindings=[]},registerListener:function(t,e,n,s){if(!(i.is(t,"function")||i.is(t,"object")&&i.is(t.handleEvent,"function")))throw new Error("listener is a required param of add() and addOnce() and should be a Function or an object implementing the EventListener interface.");var r,h;if(r=this.indexOfListener(t,n),h=this.bindings[r]){if(h.isOnce!==e)throw new Error("You cannot add"+(e?"":"Once")+"() then add"+(e?"Once":"")+"() the same listener without removing the relationship first.")}else h=new this.Binding(this,t,e,n,s),this.addBinding(h);return h},addBinding:function(i){var t=this.bindings,e=t.length;do{--e}while(t[e]&&i.priority<=t[e].priority);t.splice(e+1,0,i)},indexOfListener:function(i,t){for(var e=this.bindings,n=e.length;n--;)if(e[n].listener===i&&(void 0===t||e[n].context===t))return n;return-1},add:function(i,t,e){return this.registerListener(i,!1,t,e)},addOnce:function(i,t,e){return this.registerListener(i,!0,t,e)},remove:function(t,e){var n,s;if(!(i.is(t,"function")||i.is(t,"object")&&i.is(t.handleEvent,"function")))throw new Error("listener is a required param of remove() and should be a Function or an object implementing the EventListener interface.");if(-1!==(n=this.indexOfListener(t,e)))if(s=this.bindings[n],this.dispatching&&!s.isOnce){var r=this.bindings.indexOf(s);-1!==r&&this.bindings.splice(r,1)}else s.destroy();return t},removeAll:function(i){var t,e=this.bindings,n=e.length;if(i)for(;n--;)(t=e[n]).context===i&&t.destroy();else{for(;n--;)e[n].destroy();e.length=0}},getNumListeners:function(){return this.bindings.length},getListeners:function(){return this.bindings.map(function(i){return i.listener})},halt:function(){this.shouldPropagate=!1},dispatch:function(i,e){var n,s;if(this.active){i=t.toArray(i),s=this.bindings.slice(),this.shouldPropagate=!0,this.dispatching++;try{for(n=s.length-1;n>=0&&!1!==s[n].execute(i,e)&&this.shouldPropagate;n--);}finally{if(this.dispatching--,this.bindings)for(n=0;n<s.length;n++)this.bindings.indexOf(s[n])<0&&s[n].destroy()}}},dispose:function(){this.removeAll(),this.active=!1,delete this.bindings},toString:function(){return"[Dispatcher active: "+this.active+" numListeners: "+this.getNumListeners()+"]"}});return n.Binding=n.prototype.Binding=e.extend({listener:null,isOnce:!1,context:null,dispatcher:null,priority:0,active:!0,init:function(i,t,e,n,s){this.listener=t,this.isOnce=e,this.context=n,this.dispatcher=i,this.priority=s||0},execute:function(t,e){var n,s=this.listener,r=i.is(this.context)?this.context:e;return this.active&&(this.isOnce&&this.detach(),n="function"==typeof s.handleEvent?s.handleEvent.apply(void 0===r?s:r,t||[]):s.apply(r,t||[])),n},detach:function(){return this.dispatcher&&this.dispatcher.remove(this.listener,this.context),this.listener},getListener:function(){return this.listener},dispose:function(){this.destroy()},destroy:function(){var i,t=this.dispatcher;t&&(i=t.bindings.indexOf(this),this.active=!1,-1!==i&&t.bindings.splice(i,1),delete this.dispatcher),delete this.isOnce,delete this.listener,delete this.context},toString:function(){return"[Dispatcher.Binding isOnce: "+this.isOnce+", active: "+this.active+"]"}}),i.namespace("Dispatcher",n,i)});
define("UWA/Ajax",["UWA/Core","UWA/Utils","UWA/String"],function(e,t,r){"use strict";var n={getRequest:function(r,o){var s,a,i,u=(o=e.merge(o||{},{url:r,method:"GET",async:!0,responseType:"text",onComplete:function(){},onFailure:function(e){throw e},onTimeout:function(e){throw e},onCancel:function(){}})).method||"GET",p=o.headers||{},d=o.authentication,c=n.onStateChange;if(/OPTIONS|GET|HEAD|POST|PUT|DELETE|TRACE|CONNECT/i.test(u)&&(u=u.toUpperCase()),o.data&&(e.is(o.data,["string","arraybufferview","formdata","blob"])||(o.data=t.toQueryString(o.data)),"GET"===u&&(r+=(r.indexOf("?")>-1?"&":"?")+o.data,o.url=r,delete o.data)),o.cors||(t.getOwnPropertyMatchName(p,"X-Requested-With")||(p["X-Requested-With"]="XMLHttpRequest"),t.getOwnPropertyMatchName(p,"X-Requested-Method")||(p["X-Requested-Method"]=u)),"POST"!==u||t.getOwnPropertyMatchName(p,"Content-Type")||e.is(o.data,["arraybufferview","formdata","blob"])||(p["Content-Type"]="application/x-www-form-urlencoded; charset=utf-8"),d&&(d.username&&d.password?(i=r.split("://"),r=i[0]+"://"+d.username+":"+d.password+"@"+i[1]):r+=(r.indexOf("?")>-1?"&":"?")+t.toQueryString(d)),a=o.cors?n.createCORSRequest():n.createRequest()){if(a.cancel=function(){a.aborted=!0,a.abort()},a.addEventListener&&o.onProgress&&a.addEventListener("progress",function(e){o.onProgress(e)}),a.open(u,r,o.async),o.responseTypeSupport="responseType"in a&&"json"!==o.responseType&&(o.async||"undefined"==typeof window),o.responseTypeSupport)try{a.responseType=o.responseType}catch(e){a.responseType="text"}if(o.withCredentialsSupport="withCredentials"in a&&(o.async||"undefined"==typeof window),o.withCredentials){if(!o.withCredentialsSupport)return void o.onFailure(new Error("XMLHttpRequest does not support withCredentials."));a.withCredentials=o.withCredentials}if(o.timeout&&(a.timeoutTimer=setTimeout(function(){a.timedout=!0,a.abort()},o.timeout)),o.cors?(a.onerror=function(){e.merge(a,{readyState:4,status:500}),c(a,o)},a.onload=function(){e.merge(a,{readyState:4,status:200}),c(a,o)}):a.onreadystatechange=c.bind(n,a,o),a.setRequestHeader)for(s in p)p.hasOwnProperty(s)&&a.setRequestHeader(s,p[s]);return a}o.onFailure(new Error("Unable to initiate XMLHttpRequest object."))},createRequest:function(){var e;return window.XMLHttpRequest?e=new window.XMLHttpRequest:window.ActiveXObject&&(e=new window.ActiveXObject("Msxml2.XMLHTTP")),e},createCORSRequest:function(){var e;return window.XMLHttpRequest&&!(e=new window.XMLHttpRequest).withCredentials&&window.XDomainRequest&&(e=new window.XDomainRequest),e},request:function(e,t){var r;return t=t||{},(r=n.getRequest(e,t)).send(t.data||null),t.async||n.onStateChange(r,t),r},parseResponseHeaders:function(e){var t,r,n,o,s,a,i={};if(e)for(a=e.split("\r\n"),t=0;t<a.length;t++)(r=(s=a[t]).indexOf(": "))>0&&(n=s.substring(0,r),o=s.substring(r+2),i[n]=o);return i},onStateChange:function(){var o="UWA_Platform_";function s(t){var n,s=t;if(e.is(s,"string")&&s.contains(o))try{s=r.stripComments(s),s=JSON.parse(s)}catch(e){s=!1}if(s&&s.error&&String(s.error.type).startsWith(o))return n=new Error(r.format("ProxyError: {0}",s.error.message)),e.merge(n,s.error),n}function a(e,t){var n,o,a=t.responseTypeSupport?e.responseType:t.responseType;if(t.responseTypeSupport){if("text"===a||""===a)n=e.responseText;else try{n=e.response}catch(t){throw new Error(r.format('InvalidResponseError: request has probably invalid "Content-type" header require by responseType "{0}" causing: "{1}".',e.responseType,t))}if(t.fromDataRequest&&(o=s(n)),o)throw o}else{if(t.fromDataRequest&&(o=s(e.responseText)),o)throw o;"text"===a||""===a?n=e.responseText:"json"===a?0===(n=String(e.responseText).trim()).length?n=null:(n=r.stripComments(n),n=JSON.parse(n)):"document"===a?n=e.responseXML:"arraybuffer"===a?n=function(e){var t,r,n=new ArrayBuffer(2*e.length),o=new Uint16Array(n);for(t=0,r=e.length;t<r;t++)o[t]=e.charCodeAt(t);return n}(e.responseText):"blob"===a&&(n=new Blob([e.responseText],{type:e.getResponseHeader("Content-Type")}))}return n}function i(e){return n.parseResponseHeaders(e.getAllResponseHeaders())}return function(e,n){var s,u,p,d;if(e.aborted)n.onCancel(e,n);else if(e.timedout)n.onTimeout(new Error("Request timed out after "+n.timeout+" ms"),e,n);else if(4===e.readyState){if(e.timeoutTimer&&clearTimeout(e.timeoutTimer),e.completed)return;e.completed=!0;var c=!0;if(e.status<=0){var l=t.parseUrl(t.buildUrl(window.location,n.url)).protocol;c="http"!==l&&"https"!==l}else e.status>=400&&(c=!1);if(c){u=i(e);try{s=a(e,n)}catch(e){p=e,String(e.type).startsWith(o)&&(u=e.headers,s=e.body),n.onFailure(e,s,u)}finally{p||n.onComplete(s,u)}}else{d=new Error(r.format('NetworkError: url "{0}" return ResponseCode with value "{1}".',n.fromDataRequest||n.url,e.status||0)),u=i(e);try{s=a(e,n)}catch(e){String(e.type).startsWith(o)&&(Object.assign(d,e),u=e.headers,s=e.body)}n.onFailure(d,s,u)}!function(e,t){t.cors?(e.onerror=null,e.onload=null):e.onreadystatechange=null}(e,n)}}}()};return e.namespace("Ajax",n,e)});
define("UWA/Json",["UWA/Core","UWA/String","UWA/Utils","UWA/Utils/Client","UWA/Ajax"],function(UWA,UWAString,Utils,Client,Ajax){"use strict";var Json={jsonp:{},encode:JSON.stringify,decode:JSON.parse,prune:function(e,t){var r=[],n=t&&t.toJSON||function(e){return UWA.is(e)&&UWA.is(e.toJSON,"function")?e.toJSON():e},a=t&&t.fallback||function(){return null};return function e(t){var o,s;switch(t=n(t),UWA.typeOf(t)){case"string":case"number":case"boolean":return t;case"array":return-1!==r.indexOf(t)?a(t,"circular"):(r.push(t),o=t.map(e),r.pop(),o);case"object":if(!UWA.is(t,"plain"))return a(t,"unsupported");if(-1!==r.indexOf(t))return a(t,"circular");for(s in r.push(t),o={},t)UWA.owns(t,s)&&(o[s]=e(t[s]));return r.pop(),o;default:return null===t?t:a(t,"unsupported")}}(e)},isJson:function(e){var t=!1;if(UWA.is(e,"string"))try{JSON.parse(e),t=!0}catch(e){}return t},xmlToJson:function(e){var t,r,n,a,o,s,i=function(){return this.nodeValue},l=function(){return parseInt(this.nodeValue,10)};if("string"==typeof e&&(e=Utils.loadXml(e)),e.attributes&&0!==e.attributes.length||!e.childNodes||1!==e.childNodes.length||-1===e.childNodes[0].nodeName.indexOf("#")){if(n={},e.attributes)for(t=0,r=e.attributes.length;t<r;t++)n[s=(o=e.attributes[t]).nodeName]?(n[s]=Utils.splat(n[s]),n[s].push(o.nodeValue)):n[s]=o.nodeValue;for(t=0,r=e.childNodes.length;t<r;t++)n[s=(a=e.childNodes[t]).nodeName]?(n[s]=Utils.splat(n[s]),n[s].push(Json.xmlToJson(a))):-1===s.indexOf("#")?n[s]=Json.xmlToJson(a):a.nodeValue.trim().length>0&&(n.nodeValue=a.nodeValue,n.toString=i,n.valueOf=l)}else n=e.childNodes[0].nodeValue;return n},path:function(){var valueStr="VALUE",pathStr="PATH",sepStr=";",queryPath="$",regExps=[/[\['](\??\(.*?\))[\]']|\['(.*?)'\]/g,/'?\.'?|\['?/g,/;;;|;;/g,/;$|'?\]|'$/g,/#([0-9]+)/g,/^\$;?/,/(^|[^\\])@/g,/\\@/g,/^[0-9*]+$/,/^(-?[0-9]*):(-?[0-9]*):?(-?[0-9]*)$/g,/^\(.*?\)$/,/^\?\(.*?\)$/,/^\?\((.*?)\)$/,/^(-?[0-9]*):(-?[0-9]*):?([0-9]*)$/,/,/,/'?,'?/];function normalize(e){var t=[];return e.replace(regExps[0],function(e,r,n){return"[#"+(t.push(r||n)-1)+"]"}).replace(regExps[1],sepStr).replace(regExps[2],";..;").replace(regExps[3],"").replace(regExps[4],function(e,r){return t[r]}).replace(regExps[5],"")}function run(obj,query,val){var queryEval="var valueEval = arguments[2];"+query.replace(regExps[6],"$1valueEval").replace(regExps[7],"@");try{return obj&&val&&eval(queryEval)}catch(e){throw new SyntaxError("UWA.Json.path error: "+e.message+' for query "'+query+'"')}}function asPath(e){var t,r,n=e.split(sepStr),a=queryPath;for(t=1,r=n.length;t<r;t++)a+=regExps[8].test(n[t])?"["+n[t]+"]":"['"+n[t]+"']";return a}function store(e,t,r,n){return e&&(r[r.length]=n===pathStr?asPath(e):t),Boolean(e)}function walk(e,t,r,n,a){var o,s,i,l=UWA.typeOf(r);if("array"===l)for(o=0,s=r.length;o<s;o++)r.hasOwnProperty(o)&&a(o,e,t,r,n);else if("object"===l)for(i in r)r.hasOwnProperty(i)&&a(i,e,t,r,n)}function slice(e,t,r,n,a,o){if(Array.isArray(r)){var s,i=r.length,l=0,u=1,c=i;for(e.replace(regExps[9],function(e,t,r,n){l=parseInt(t||l,10),c=parseInt(r||c,10),u=parseInt(n||u,10)}),l=l<0?Math.max(0,l+i):Math.min(i,l),c=c<0?Math.max(0,c+i):Math.min(i,c),s=l;s<c;s+=u)trace(s+sepStr+t,r,n,a,o)}}function trace(e,t,r,n,a){if(""!==e){var o,s,i,l=e.split(sepStr),u=l.shift();if(l=l.join(sepStr),t&&t.hasOwnProperty(u))trace(l,t[u],r+sepStr+u,n,a);else if("*"===u)walk(u,l,t,r,function(e,t,r,o,s){trace(e+sepStr+r,o,s,n,a)});else if(".."===u)trace(l,t,r,n,a),walk(u,l,t,r,function(e,t,r,o,s){"object"==typeof o[e]&&trace("..;"+r,o[e],s+sepStr+e,n,a)});else if(regExps[10].test(u))trace(e=run(t,u,t,r.substr(r.lastIndexOf(sepStr)+1))+sepStr+l,t,r,n,a);else if(regExps[11].test(u))walk(u,l,t,r,function(e,r,o,s,i){run(t,r.replace(regExps[12],"$1"),Array.isArray(s)?s[e]:s,e)&&trace(e+sepStr+o,s,i,n,a)});else if(regExps[13].test(u))slice(u,l,t,r,n,a);else if(regExps[14].test(u))for(s=0,i=(o=u.split(regExps[15])).length;s<i;s++)trace(e=o[s]+sepStr+l,t,r,n,a)}else store(r,t,n,a)}return function(e,t,r){var n=[],a=r&&r.resultType||valueStr;return e&&t&&(a===valueStr||a===pathStr)&&trace(normalize(t),e,queryPath,n,a),!!n.length&&n}}(),request:function(e,t){var r,n,a,o,s,i,l,u,c,p,f,d,m,h=!!(t=t||{}).useJsonpRequest||!Utils.matchUrl(e,window.location)&&(UWA.Data&&UWA.Data.useJsonpRequest&&!UWA.Data.allowCrossOriginRequest),g=e,v=Client.isOnline,w=Json.jsonp,y={fromDataRequest:!1,useOfflineCache:!1,async:!0,timeout:!1,callback:"jsonp"+(Date.now()+Utils.random(1,1e4)),callbackName:"callback",callbackMode:"function",callbackModeName:"callbackMode",onCancel:function(){},onFailure:function(e){throw e},onComplete:function(){}};if(!1===(t=UWA.merge(t||{},y)).timeout?t.useOfflineCache?t.timeout=15e3:t.timeout=25e3:t.timeout=parseInt(t.timeout,10),t.data&&(e+=(e.indexOf("?")>-1?"&":"?")+Utils.toQueryString(t.data)),n=t.callback.replace(/[^a-zA-Z0-9_]/g,"$"),(a=t.callbackMode)&&(e=e.replace(/\=(\?|%3F)/g,"="+n),e+=(e.indexOf("?")>-1?"&":"?")+t.callbackName+"="+n,e+="&"+t.callbackModeName+"="+a),e.length>2048)throw new Error("Proxified url is more than 2048 characters, you should consider using POST and CORS Ajax.");return o=t.onFailure,i=t.onTimeout||o,s=t.onComplete,l=t.useOfflineCache,u=t.fromDataRequest,t.onFailure=function(e){if(Json.cleanRequest(n,t),l&&!1===u){var r=Json.getFromCache(g);UWA.is(r)?(v()&&v(!1,5e3),s(r)):o(e)}else o(e)},t.onTimeout=function(e){if(Json.cleanRequest(n,t),l&&!1===u){var r=Json.getFromCache(g);UWA.is(r)?(v()&&v(!1,5e3),s(r)):i(e)}else i(e)},t.onComplete=function(e){Json.cleanRequest(n,t);try{if(u&&e&&e.error&&e.error.type&&"UWA_Platform_Exposition"===e.error.type)throw new Error(UWAString.format('ObjectError: url "{0}" return Error with value "{1}"',u,e.error.message||e.error));s(e)}catch(e){o(e)}},t.cache<0&&(e+=(e.indexOf("?")>-1?"&":"?")+"_="+Date.now()),l&&!1===v()?t.onFailure(new Error("Network is Offline")):h?(w[n]={readyState:!1,options:t},"object"===a?(f=Date.now(),d=13,m=function(){var e,r=Date.now();void 0!==window[n]?(w[n].readyState="loaded",t.onComplete(window[n])):r>f+t.timeout?(e=r-f,t.onTimeout(new Error("Request timed out after "+e+"ms with timeout value "+t.timeout+" ms"))):w[n].poll=setTimeout(m.bind(this),d)}):(window[n]=function(e){void 0!==w[n]&&(w[n].data=e,w[n].readyState="loaded")},f=Date.now(),d=13,m=function(){var e,r=Date.now();"loaded"===w[n].readyState?t.onComplete(w[n].data):r>f+t.timeout?(e=r-f,t.onTimeout(new Error("Timout request after "+e+"ms with timeout value "+t.timeout+" ms"))):w[n].poll=setTimeout(m.bind(this),d)}),c=document.getElementsByTagName("head")[0],(p=UWA.createElement("script",{type:"text/javascript",src:e,async:t.async})).addEvent("error",function(){t.onFailure(new Error("Syntax or http error: "+e))}),p.inject(c),w[n].script=p,m(t),r={jsonId:n,script:p,cancel:function(){w[n].aborted=!0,Json.cleanRequest(n)}}):r=Ajax.request(e,UWA.merge({headers:{Accept:"application/json,text/javascript,*/*","X-Request":"JSON"},onComplete:function(e){var r;a&&!Json.isJson(e)&&((r="object"===a?e.match(/=\s\(?([\s\S]*?)\)?;?\s*$/):e.match(/\(([\s\S]*?)\);?\s*$/))&&(e=r[1]));Json.isJson(e)?t.onComplete(UWA.Json.decode(e)):t.onFailure(new Error('Invalid JSON Response: "'+e+'"'))},onFailure:t.onFailure},t)),r},cleanRequest:function(e){var t,r=document.getElementsByTagName("head")[0],n=Json.jsonp[e];n&&(t=n.options,clearTimeout(n.poll),"object"!==t.callbackMode&&(window[e]=function(){try{delete window[e]}catch(e){}}),n.script&&(r.removeChild(n.script),delete n.script),n.aborted&&t.onCancel(null,t))}};return UWA.namespace("Json",Json,UWA)});
define("UWA/Event",["UWA/Core"],function(e){"use strict";var t,n,a={onDomReady:function(e,t){t=t||window;var n=!1,a=!0,o=window.document,c=o.documentElement,r=Boolean(o.addEventListener),l=r?"addEventListener":"attachEvent",i=r?"removeEventListener":"detachEvent",u=r?"":"on";function d(a){var c=a.type;"complete"!==o.readyState&&"interactive"!==o.readyState||(o[i](u+"DOMContentLoaded",d,!1),o[i](u+"readystatechange",d,!1),window[i](u+"load",d,!1),n||(n=!0,e.call(t,c||a)))}if("complete"===o.readyState)setTimeout(e.bind(t,"lazy"),1);else{if(o.createEventObject&&c.doScroll){try{a=!window.frameElement}catch(e){}a&&function e(){try{c.doScroll("left"),d("poll")}catch(t){setTimeout(e,50)}}()}o[l](u+"DOMContentLoaded",d,!1),o[l](u+"readystatechange",d,!1),window[l](u+"load",d,!1)}},dispatchEvent:function(t,n,a){var o,c,r,l=9===t.nodeType?t:t.ownerDocument||t.document,i={canBubble:!0,cancelable:!0,view:l.defaultView||l.parentWindow,ctrlKey:!1,altKey:!1,shiftKey:!1,metaKey:!1,detail:0,screenX:0,screenY:0,clientX:0,clientY:0,button:0,relatedTarget:null,keyCode:null,charCode:null,touches:null,targetTouches:null,changedTouches:null,scale:1,rotation:0};if(a=e.merge(a||{},i),l.createEvent){if("click"===n||"dblclick"===n||"contextmenu"===n||0===n.indexOf("mouse")?(c="MouseEvent",r=[n,a.canBubble,a.cancelable,a.view,a.detail,a.screenX,a.screenY,a.clientX,a.clientY,a.ctrlKey,a.altKey,a.shiftKey,a.metaKey,a.button,a.relatedTarget]):0===n.indexOf("touch")?(c="TouchEvent",r=[n,a.canBubble,a.cancelable,a.view,a.detail,a.screenX,a.screenY,a.clientX,a.clientY,a.ctrlKey,a.altKey,a.shiftKey,a.metaKey,a.touches,a.targetTouches,a.changedTouches,a.scale,a.rotation]):0===n.indexOf("key")?(c="KeyboardEvent",r=[n,a.canBubble,a.cancelable,a.view,a.ctrlKey,a.altKey,a.shiftKey,a.metaKey,a.keyCode,a.charCode]):(c="HTMLEvents",r=[n,a.canBubble,a.cancelable]),o=l.createEvent(c),"KeyboardEvent"===c&&"function"==typeof o.initKeyEvent?c="KeyEvent":"HTMLEvents"===c&&"function"!=typeof o.initHTMLEvents&&(c="Event"),"function"!=typeof o["init"+c])throw new Error("Unsuported Event type "+c);o["init"+c].apply(o,r),t.dispatchEvent(o)}else if(l.createEventObject){o=l.createEventObject(),e.extend(o,a);try{t.fireEvent("on"+n,o)}catch(e){throw new Error("Unsuported Event type "+n)}}return o},getElement:function(t){var n=t._uwaTarget||t.target||t.srcElement;return"DOMCharacterDataModified"===t.type||!n||3!==n.nodeType&&4!==n.nodeType||(n=n.parentNode),e.extendElement(n)},findElement:function(e,t){return a.getElement(e).getClosest(t)},getPosition:function(e,t){var n;"number"==typeof t?t={touchIndex:t}:t||(t={});var a=e.changedTouches||e.touches,o="client"===t.relativeTo,c=o?"clientX":"pageX",r=o?"clientY":"pageY";if(a)if(void 0!==t.touchIndex&&a[t.touchIndex])n={x:a[t.touchIndex][c],y:a[t.touchIndex][r]};else{n={x:0,y:0};for(var l=0,i=a.length;l<i;l++)n.x+=a[l][c],n.y+=a[l][r];n.x/=i,n.y/=i}else n={x:e[c],y:e[r]};return n},stopPropagation:function(e){e.stopPropagation&&e.stopPropagation(),e.cancelBubble=!0},preventDefault:function(e){e.preventDefault&&e.preventDefault(),e.returnValue=!1,void 0!==e.cancelable&&!0!==e.cancelable||void 0!==e.defaultPrevented||(e.defaultPrevented=!0)},stop:function(e){a.preventDefault(e),a.stopPropagation(e)},isDefaultPrevented:function(e){return e.defaultPrevented||!0!==e.returnValue&&void 0!==e.returnValue},whichButton:function(t){var n=t.button,a=t.which;return!a&&e.is(n)&&(a=[0,1,3,1,2][n]||0),a-1},whichKey:(t=["alt","ctrl","meta","shift"],n={8:"backspace",9:"tab",13:"return",16:"shift",17:"ctrl",18:"alt",19:"pause",20:"capslock",27:"esc",32:"space",33:"pageup",34:"pagedown",35:"end",36:"home",37:"left",38:"up",39:"right",40:"down",45:"insert",46:"del",96:"0",97:"1",98:"2",99:"3",100:"4",101:"5",102:"6",103:"7",104:"8",105:"9",106:"*",107:"+",109:"-",110:".",111:"/",112:"f1",113:"f2",114:"f3",115:"f4",116:"f5",117:"f6",118:"f7",119:"f8",120:"f9",121:"f10",122:"f11",123:"f12",144:"numlock",145:"scroll",191:"/",224:"meta"},function(e){var a,o,c,r=e.which||e.keyCode,l="keypress"!==e.type&&n[r],i=[];for(a=0,o=t.length;a<o;a++)e[(c=t[a])+"Key"]&&l!==c&&i.push(c);return l?i.push(l):r&&0===e.type.indexOf("key")&&i.push(String.fromCharCode(r).toLowerCase()),i.join("+")}),wheelDelta:function(e){return e.wheelDelta?e.wheelDelta/120:-(e.detail||0)/3}};return e.namespace("Event",a,e)});

define('vendors/webcomponents/WeakMap', [],function () {
    /*
 * Copyright 2012 The Polymer Authors. All rights reserved.
 * Use of this source code is governed by a BSD-style
 * license that can be found in the LICENSE file.
 */

if (typeof WeakMap === 'undefined') {
  (function() {
    var defineProperty = Object.defineProperty;
    var counter = Date.now() % 1e9;

    var WeakMap = function() {
      this.name = '__st' + (Math.random() * 1e9 >>> 0) + (counter++ + '__');
    };

    WeakMap.prototype = {
      set: function(key, value) {
        var entry = key[this.name];
        if (entry && entry[0] === key)
          entry[1] = value;
        else
          defineProperty(key, this.name, {value: [key, value], writable: true});
        return this;
      },
      get: function(key) {
        var entry;
        return (entry = key[this.name]) && entry[0] === key ?
            entry[1] : undefined;
      },
      'delete': function(key) {
        var entry = key[this.name];
        if (!entry || entry[0] !== key) return false;
        entry[0] = entry[1] = undefined;
        return true;
      },
      has: function(key) {
        var entry = key[this.name];
        if (!entry) return false;
        return entry[0] === key;
      }
    };

    window.WeakMap = WeakMap;
  })();
};
    return window.WeakMap;
});



define('vendors/webcomponents/MutationObserver', ['./WeakMap'], function () {
    /*
 * Copyright 2012 The Polymer Authors. All rights reserved.
 * Use of this source code is goverened by a BSD-style
 * license that can be found in the LICENSE file.
 */

(function(global) {

  var registrationsTable = new WeakMap();

  var setImmediate;

  // As much as we would like to use the native implementation, IE
  // (all versions) suffers a rather annoying bug where it will drop or defer
  // callbacks when heavy DOM operations are being performed concurrently.
  //
  // For a thorough discussion on this, see:
  // http://codeforhire.com/2013/09/21/setimmediate-and-messagechannel-broken-on-internet-explorer-10/
  if (/Trident/.test(navigator.userAgent)) {
    // Sadly, this bug also affects postMessage and MessageQueues.
    //
    // We would like to use the onreadystatechange hack for IE <= 10, but it is
    // dangerous in the polyfilled environment due to requiring that the
    // observed script element be in the document.
    setImmediate = setTimeout;

  // If some other browser ever implements it, let's prefer their native
  // implementation:
  } else if (window.setImmediate) {
    setImmediate = window.setImmediate;

  // Otherwise, we fall back to postMessage as a means of emulating the next
  // task semantics of setImmediate.
  } else {
    var setImmediateQueue = [];
    var sentinel = String(Math.random());
    window.addEventListener('message', function(e) {
      if (e.data === sentinel) {
        var queue = setImmediateQueue;
        setImmediateQueue = [];
        queue.forEach(function(func) {
          func();
        });
      }
    });
    setImmediate = function(func) {
      setImmediateQueue.push(func);
      window.postMessage(sentinel, '*');
    };
  }

  // This is used to ensure that we never schedule 2 callas to setImmediate
  var isScheduled = false;

  // Keep track of observers that needs to be notified next time.
  var scheduledObservers = [];

  /**
   * Schedules |dispatchCallback| to be called in the future.
   * @param {MutationObserver} observer
   */
  function scheduleCallback(observer) {
    scheduledObservers.push(observer);
    if (!isScheduled) {
      isScheduled = true;
      setImmediate(dispatchCallbacks);
    }
  }

  function wrapIfNeeded(node) {
    return window.ShadowDOMPolyfill &&
        window.ShadowDOMPolyfill.wrapIfNeeded(node) ||
        node;
  }

  function dispatchCallbacks() {
    // http://dom.spec.whatwg.org/#mutation-observers

    isScheduled = false; // Used to allow a new setImmediate call above.

    var observers = scheduledObservers;
    scheduledObservers = [];
    // Sort observers based on their creation UID (incremental).
    observers.sort(function(o1, o2) {
      return o1.uid_ - o2.uid_;
    });

    var anyNonEmpty = false;
    observers.forEach(function(observer) {

      // 2.1, 2.2
      var queue = observer.takeRecords();
      // 2.3. Remove all transient registered observers whose observer is mo.
      removeTransientObserversFor(observer);

      // 2.4
      if (queue.length) {
        observer.callback_(queue, observer);
        anyNonEmpty = true;
      }
    });

    // 3.
    if (anyNonEmpty)
      dispatchCallbacks();
  }

  function removeTransientObserversFor(observer) {
    observer.nodes_.forEach(function(node) {
      var registrations = registrationsTable.get(node);
      if (!registrations)
        return;
      registrations.forEach(function(registration) {
        if (registration.observer === observer)
          registration.removeTransientObservers();
      });
    });
  }

  /**
   * This function is used for the "For each registered observer observer (with
   * observer's options as options) in target's list of registered observers,
   * run these substeps:" and the "For each ancestor ancestor of target, and for
   * each registered observer observer (with options options) in ancestor's list
   * of registered observers, run these substeps:" part of the algorithms. The
   * |options.subtree| is checked to ensure that the callback is called
   * correctly.
   *
   * @param {Node} target
   * @param {function(MutationObserverInit):MutationRecord} callback
   */
  function forEachAncestorAndObserverEnqueueRecord(target, callback) {
    for (var node = target; node; node = node.parentNode) {
      var registrations = registrationsTable.get(node);

      if (registrations) {
        for (var j = 0; j < registrations.length; j++) {
          var registration = registrations[j];
          var options = registration.options;

          // Only target ignores subtree.
          if (node !== target && !options.subtree)
            continue;

          var record = callback(options);
          if (record)
            registration.enqueue(record);
        }
      }
    }
  }

  var uidCounter = 0;

  /**
   * The class that maps to the DOM MutationObserver interface.
   * @param {Function} callback.
   * @constructor
   */
  function JsMutationObserver(callback) {
    this.callback_ = callback;
    this.nodes_ = [];
    this.records_ = [];
    this.uid_ = ++uidCounter;
  }

  JsMutationObserver.prototype = {
    observe: function(target, options) {
      target = wrapIfNeeded(target);

      // 1.1
      if (!options.childList && !options.attributes && !options.characterData ||

          // 1.2
          options.attributeOldValue && !options.attributes ||

          // 1.3
          options.attributeFilter && options.attributeFilter.length &&
              !options.attributes ||

          // 1.4
          options.characterDataOldValue && !options.characterData) {

        throw new SyntaxError();
      }

      var registrations = registrationsTable.get(target);
      if (!registrations)
        registrationsTable.set(target, registrations = []);

      // 2
      // If target's list of registered observers already includes a registered
      // observer associated with the context object, replace that registered
      // observer's options with options.
      var registration;
      for (var i = 0; i < registrations.length; i++) {
        if (registrations[i].observer === this) {
          registration = registrations[i];
          registration.removeListeners();
          registration.options = options;
          break;
        }
      }

      // 3.
      // Otherwise, add a new registered observer to target's list of registered
      // observers with the context object as the observer and options as the
      // options, and add target to context object's list of nodes on which it
      // is registered.
      if (!registration) {
        registration = new Registration(this, target, options);
        registrations.push(registration);
        this.nodes_.push(target);
      }

      registration.addListeners();
    },

    disconnect: function() {
      this.nodes_.forEach(function(node) {
        var registrations = registrationsTable.get(node);
        for (var i = 0; i < registrations.length; i++) {
          var registration = registrations[i];
          if (registration.observer === this) {
            registration.removeListeners();
            registrations.splice(i, 1);
            // Each node can only have one registered observer associated with
            // this observer.
            break;
          }
        }
      }, this);
      this.records_ = [];
    },

    takeRecords: function() {
      var copyOfRecords = this.records_;
      this.records_ = [];
      return copyOfRecords;
    }
  };

  /**
   * @param {string} type
   * @param {Node} target
   * @constructor
   */
  function MutationRecord(type, target) {
    this.type = type;
    this.target = target;
    this.addedNodes = [];
    this.removedNodes = [];
    this.previousSibling = null;
    this.nextSibling = null;
    this.attributeName = null;
    this.attributeNamespace = null;
    this.oldValue = null;
  }

  function copyMutationRecord(original) {
    var record = new MutationRecord(original.type, original.target);
    record.addedNodes = original.addedNodes.slice();
    record.removedNodes = original.removedNodes.slice();
    record.previousSibling = original.previousSibling;
    record.nextSibling = original.nextSibling;
    record.attributeName = original.attributeName;
    record.attributeNamespace = original.attributeNamespace;
    record.oldValue = original.oldValue;
    return record;
  };

  // We keep track of the two (possibly one) records used in a single mutation.
  var currentRecord, recordWithOldValue;

  /**
   * Creates a record without |oldValue| and caches it as |currentRecord| for
   * later use.
   * @param {string} oldValue
   * @return {MutationRecord}
   */
  function getRecord(type, target) {
    return currentRecord = new MutationRecord(type, target);
  }

  /**
   * Gets or creates a record with |oldValue| based in the |currentRecord|
   * @param {string} oldValue
   * @return {MutationRecord}
   */
  function getRecordWithOldValue(oldValue) {
    if (recordWithOldValue)
      return recordWithOldValue;
    recordWithOldValue = copyMutationRecord(currentRecord);
    recordWithOldValue.oldValue = oldValue;
    return recordWithOldValue;
  }

  function clearRecords() {
    currentRecord = recordWithOldValue = undefined;
  }

  /**
   * @param {MutationRecord} record
   * @return {boolean} Whether the record represents a record from the current
   * mutation event.
   */
  function recordRepresentsCurrentMutation(record) {
    return record === recordWithOldValue || record === currentRecord;
  }

  /**
   * Selects which record, if any, to replace the last record in the queue.
   * This returns |null| if no record should be replaced.
   *
   * @param {MutationRecord} lastRecord
   * @param {MutationRecord} newRecord
   * @param {MutationRecord}
   */
  function selectRecord(lastRecord, newRecord) {
    if (lastRecord === newRecord)
      return lastRecord;

    // Check if the the record we are adding represents the same record. If
    // so, we keep the one with the oldValue in it.
    if (recordWithOldValue && recordRepresentsCurrentMutation(lastRecord))
      return recordWithOldValue;

    return null;
  }

  /**
   * Class used to represent a registered observer.
   * @param {MutationObserver} observer
   * @param {Node} target
   * @param {MutationObserverInit} options
   * @constructor
   */
  function Registration(observer, target, options) {
    this.observer = observer;
    this.target = target;
    this.options = options;
    this.transientObservedNodes = [];
  }

  Registration.prototype = {
    enqueue: function(record) {
      var records = this.observer.records_;
      var length = records.length;

      // There are cases where we replace the last record with the new record.
      // For example if the record represents the same mutation we need to use
      // the one with the oldValue. If we get same record (this can happen as we
      // walk up the tree) we ignore the new record.
      if (records.length > 0) {
        var lastRecord = records[length - 1];
        var recordToReplaceLast = selectRecord(lastRecord, record);
        if (recordToReplaceLast) {
          records[length - 1] = recordToReplaceLast;
          return;
        }
      } else {
        scheduleCallback(this.observer);
      }

      records[length] = record;
    },

    addListeners: function() {
      this.addListeners_(this.target);
    },

    addListeners_: function(node) {
      var options = this.options;
      if (options.attributes)
        node.addEventListener('DOMAttrModified', this, true);

      if (options.characterData)
        node.addEventListener('DOMCharacterDataModified', this, true);

      if (options.childList)
        node.addEventListener('DOMNodeInserted', this, true);

      if (options.childList || options.subtree)
        node.addEventListener('DOMNodeRemoved', this, true);
    },

    removeListeners: function() {
      this.removeListeners_(this.target);
    },

    removeListeners_: function(node) {
      var options = this.options;
      if (options.attributes)
        node.removeEventListener('DOMAttrModified', this, true);

      if (options.characterData)
        node.removeEventListener('DOMCharacterDataModified', this, true);

      if (options.childList)
        node.removeEventListener('DOMNodeInserted', this, true);

      if (options.childList || options.subtree)
        node.removeEventListener('DOMNodeRemoved', this, true);
    },

    /**
     * Adds a transient observer on node. The transient observer gets removed
     * next time we deliver the change records.
     * @param {Node} node
     */
    addTransientObserver: function(node) {
      // Don't add transient observers on the target itself. We already have all
      // the required listeners set up on the target.
      if (node === this.target)
        return;

      this.addListeners_(node);
      this.transientObservedNodes.push(node);
      var registrations = registrationsTable.get(node);
      if (!registrations)
        registrationsTable.set(node, registrations = []);

      // We know that registrations does not contain this because we already
      // checked if node === this.target.
      registrations.push(this);
    },

    removeTransientObservers: function() {
      var transientObservedNodes = this.transientObservedNodes;
      this.transientObservedNodes = [];

      transientObservedNodes.forEach(function(node) {
        // Transient observers are never added to the target.
        this.removeListeners_(node);

        var registrations = registrationsTable.get(node);
        for (var i = 0; i < registrations.length; i++) {
          if (registrations[i] === this) {
            registrations.splice(i, 1);
            // Each node can only have one registered observer associated with
            // this observer.
            break;
          }
        }
      }, this);
    },

    handleEvent: function(e) {
      // Stop propagation since we are managing the propagation manually.
      // This means that other mutation events on the page will not work
      // correctly but that is by design.
      e.stopImmediatePropagation();

      switch (e.type) {
        case 'DOMAttrModified':
          // http://dom.spec.whatwg.org/#concept-mo-queue-attributes

          var name = e.attrName;
          var namespace = e.relatedNode.namespaceURI;
          var target = e.target;

          // 1.
          var record = new getRecord('attributes', target);
          record.attributeName = name;
          record.attributeNamespace = namespace;

          // 2.
          var oldValue =
              e.attrChange === MutationEvent.ADDITION ? null : e.prevValue;

          forEachAncestorAndObserverEnqueueRecord(target, function(options) {
            // 3.1, 4.2
            if (!options.attributes)
              return;

            // 3.2, 4.3
            if (options.attributeFilter && options.attributeFilter.length &&
                options.attributeFilter.indexOf(name) === -1 &&
                options.attributeFilter.indexOf(namespace) === -1) {
              return;
            }
            // 3.3, 4.4
            if (options.attributeOldValue)
              return getRecordWithOldValue(oldValue);

            // 3.4, 4.5
            return record;
          });

          break;

        case 'DOMCharacterDataModified':
          // http://dom.spec.whatwg.org/#concept-mo-queue-characterdata
          var target = e.target;

          // 1.
          var record = getRecord('characterData', target);

          // 2.
          var oldValue = e.prevValue;


          forEachAncestorAndObserverEnqueueRecord(target, function(options) {
            // 3.1, 4.2
            if (!options.characterData)
              return;

            // 3.2, 4.3
            if (options.characterDataOldValue)
              return getRecordWithOldValue(oldValue);

            // 3.3, 4.4
            return record;
          });

          break;

        case 'DOMNodeRemoved':
          this.addTransientObserver(e.target);
          // Fall through.
        case 'DOMNodeInserted':
          // http://dom.spec.whatwg.org/#concept-mo-queue-childlist
          var target = e.relatedNode;
          var changedNode = e.target;
          var addedNodes, removedNodes;
          if (e.type === 'DOMNodeInserted') {
            addedNodes = [changedNode];
            removedNodes = [];
          } else {

            addedNodes = [];
            removedNodes = [changedNode];
          }
          var previousSibling = changedNode.previousSibling;
          var nextSibling = changedNode.nextSibling;

          // 1.
          var record = getRecord('childList', target);
          record.addedNodes = addedNodes;
          record.removedNodes = removedNodes;
          record.previousSibling = previousSibling;
          record.nextSibling = nextSibling;

          forEachAncestorAndObserverEnqueueRecord(target, function(options) {
            // 2.1, 3.2
            if (!options.childList)
              return;

            // 2.2, 3.3
            return record;
          });

      }

      clearRecords();
    }
  };

  global.JsMutationObserver = JsMutationObserver;

  if (!global.MutationObserver)
    global.MutationObserver = JsMutationObserver;


})(this);;
    return window.MutationObserver;
});


define("UWA/Element",["UWA/Internal/Deprecate","UWA/Core","UWA/String","UWA/Array","UWA/Utils","UWA/Utils/Client","UWA/Dispatcher","UWA/Json","UWA/Event","vendors/webcomponents/MutationObserver"],function(t,e,n,i,r,o,a,s,l,c){"use strict";var d=Boolean("object"==typeof MooTools&&MooTools.version),h=o.getVendorProperty,u=document.documentElement,f=function(e,n){return t.warn("new Element(...)","Use Element.create instead"),f.create(e,n)};f.create=function(){return function(t,n){var i=function(t,e){var n,i;return"iframe"===t&&e&&void 0!==e.name?((n=document.createElement("div")).innerHTML="<"+t+' name="'+e.name+'"/>',i=n.firstChild,delete e.name):"object"===t&&e&&void 0!==e.classid?(e.html?(i=document.createElement("div"),f.setHTML.call(i,e.html),i=f.getHTML.call(i)):i="",(n=document.createElement("div")).innerHTML="<"+t+' classid="'+e.classid+'">'+i+"</"+t+">",i=n.firstChild,delete e.html,delete e.classid):i=document.createElement(t),i}(t,n);return f.extend(i),e.is(n,"object")&&f.set.call(i,n),i}}(),f.extend=function(){function n(e){var n="#document"===e.nodeName;for(var i in n&&t.warn("UWA.extendElement(document)"),f)f.hasOwnProperty(i)&&"create"!==i&&"extend"!==i&&(n&&i in e||(e[i]=f[i]))}var i={getProperty:window.Element.prototype.getProperty,getSize:function(){var t;return(t="body"===f.getTagName.call(this)?e.Utils.Client.getSize():f.getSize.call(this)).x=t.width,t.y=t.height,t},getCoordinates:function(t){var e=t?this.getPosition(t):this.getOffsets(),n=this.getSize(),i={left:e.x,top:e.y,width:n.x,height:n.y};return i.right=i.left+i.width,i.bottom=i.top+i.height,i}};return function(t){return t&&!t._isUwaExtended&&(d?function(t){delete t.fireEvent,n(t),e.extend(t,i)}(t):n(t),t._isUwaExtended=!0),t}}(),e.createElement=f.create,e.extendElement=f.extend;var m,g,p,v=(m=document.createElement("div"),g=/(^|,)/g,p=/(?:^|,)\s*[>+~]/,function(t,e,n,i){var r,o,a,s,l=i||p.test(e);return l?(n?(o=n.parentNode,s="uwa-private-get-element-selector-root-"+(1e8*Math.random()|0),n.setAttribute(s,"true"),r="["+s+"] ",i||o||(o=f.extend(m).grab(n))):(r="* ",o=n),e=e.replace(g,"$1"+r)):o=n,a=i?(f[t]||i[t]).call(i,e):(f[t]||o[t]).call(o,e),n&&l&&(n.removeAttribute(s),o===m&&o.removeChild(n)),a});function y(t){var e=t?t.indexOf(" "):-1;return e<0?{name:t}:{name:t.slice(0,e),selector:t.slice(e+1)}}var w,b,x,E,C,S,T,W,L=a.extend({Binding:a.Binding.extend({delegates:null,direct:!1,element:null,init:function(){this._parent.apply(this,arguments),this.delegates=[]},addDelegate:function(t){t?this.delegates.push(t):this.direct=!0},removeDelegate:function(t){t?this.delegates=this.delegates.filter(function(e){return e!==t}):this.direct=!1,this.direct||this.delegates.length||this.detach()},execute:function(t,e){var n,i,r,o;if(this.active){if(this.delegates.length)for(n=this.delegates.join(","),i=t[0],r=l.getElement(i);r&&r!==this.element&&!1!==o;)f.match.call(r,n,this.element)&&(i._uwaTarget=r,o=this._parent(t,e),i._uwaTarget=null),r=r.parentNode;this.direct&&!1!==o&&(o=this._parent(t,e))}return o},destroy:function(){this._parent(),delete this.element}}),init:function(t){this._parent(),this.element=t},addDelegation:function(t,e,n,i){var r=this.add(t,n,i);return r.addDelegate(e),r.element=this.element,r},removeDelegation:function(t,e){if(t){var n=this.bindings[this.indexOfListener(t)];n&&n.removeDelegate(e)}else i.invoke(this.bindings.slice(),"removeDelegate",e)},dispose:function(){this._parent(),delete this.element}});function O(t){var e="string"==typeof t.className?t.className:t.getAttribute("class");return e||""}function D(t,e){"string"==typeof t.className?t.className=e:t.setAttribute("class",e)}function N(t,e){"function"==typeof e?e=e():void 0===e&&(e=h(u,"on{}"+t,!0))&&(e=e.slice(2)),t!==e&&(f.Events[t]=function(n,i){if(!e)throw new Error("The event "+t+" is not supported on this platform");f.addEvent.call(i,e,n.handleEvent,!0),n.events[e]=n.handleEvent})}function H(){window.document&&(window.document.body&&e.extendElement(window.document.body),window.document.documentElement&&e.extendElement(window.document.documentElement))}return Object.assign(f,{set:function(t,i){var r,o;if(W||(W={html:f.setHTML,events:f.addEvents,id:function(t){this.id=t},class:function(t){this.className=t},value:function(t){this.value=t}},["compact","nowrap","ismap","declare","noshade","checked","disabled","readOnly","multiple","selected","noresize","defer","defaultChecked","autofocus","controls","autoplay","loop"].forEach(function(t){W[t.toLowerCase()]=function(e){this[t]=Boolean(e)}})),e.is(t,"object"))for(r in t)t.hasOwnProperty(r)&&f.set.call(this,r,t[r]);else o=f["set"+n.capitalize(t)],e.is(o,"function")?o.apply(this,Array.prototype.slice.call(arguments,1)):W.hasOwnProperty(t)&&!1!==W[t].call(this,i)||this.setAttribute(t,i);return this},setAttributes:function(t){var e;for(e in t)t.hasOwnProperty(e)&&this.setAttribute(e,t[e]);return this},getTagName:function(){var t=this.tagName||this.nodeName;return t?t.toLowerCase():""},setText:function(t){return f.empty.call(this),f.appendText.call(this,t)},appendText:function(t){var e=f.getDocument.call(this);return this.appendChild(e.createTextNode(t)),this},getText:function(){return"string"==typeof this.textContent?this.textContent:"string"==typeof this.innerText?this.innerText:""},setContent:function(){return f.empty.call(this),f.addContent.apply(this,arguments)},addContent:function(){return function(){var t=f.getDocument.call(this),n=t.createDocumentFragment();return function t(n,i,r){var o,a,s,l;for(e.is(n,"nodelist")&&(n=[].slice.call(n)),o=0,a=n.length;o<a;o++)if(l=n[o])if(l.nodeType)r.appendChild(l);else if("string"==typeof l||"number"==typeof l)if(/<|&#?\w+;/.test(l))for(s=i.createElement("div"),f.setHTML.call(s,l);s.firstChild;)r.appendChild(s.firstChild);else r.appendChild(i.createTextNode(l));else"function"!=typeof l.inject||Array.isArray(l)?"number"==typeof l.length?t(l,i,r):"object"==typeof l?(s=l.tag||"div",delete l.tag,r.appendChild(f.create(s,l)),l.tag=s):r.appendChild(i.createTextNode(l)):l.inject(r)}(arguments,t,n),this.appendChild(n),this}}(),setHTML:function(t){var i;if("string"!=typeof t)f.setContent.call(this,t);else try{i=n.escapeHTMLEntities(t).replace('<?xml version="1.0" encoding="UTF-8"?>',"").replace(/&(?!#?[a-z0-9]+;)/gi,"&#38;"),this.innerHTML=i}catch(i){e.log("UWA.Element.setHTML error cause: "+i+' with HTML value "'+t+'"');try{this.innerHTML=n.stripTags(String(t))}catch(e){f.setText.call(this,t)}}return this},getHTML:function(){var t=this.innerHTML;return o.Engine.ie&&(t=t.replace(/< *(\/ *)?(\w+)/g,function(t){return t.toLowerCase()})),t},inject:function(t,e){var n,i=f.getDocument.call(this);return"bottom"===(e=e||"bottom")?t.appendChild(this):"top"===e?t.insertBefore(this,t.firstChild):((n=t.parentNode)||11===t.nodeType||(n=i.createDocumentFragment()).appendChild(t),n&&("after"===e?n.lastChild===t?n.appendChild(this):n.insertBefore(this,t.nextSibling):"before"===e&&n.insertBefore(this,t))),this},grab:function(t,e){return f.inject.call(t,this,e),this},isInjected:u.contains?function(t){return(t=t||this.ownerDocument.documentElement)!==this&&(!t.contains||t.contains(this))}:u.compareDocumentPosition?function(t){return t=t||this.ownerDocument.documentElement,Boolean(16&t.compareDocumentPosition(this))}:function(t){var e=this;t=t||e.ownerDocument.documentElement;do{e=e.parentNode}while(e&&e.parentNode);return e===t},empty:function(t){for(var e;this.firstChild;)e=this.firstChild,t?f.destroy.call(e):this.removeChild(e);return this},remove:function(){var t=f.getParent.call(this);return t&&t.removeChild(this),this},destroy:function(){var t,e,n,i=f.remove,r=f.destroy,o=f.getChildren.call(this);for(e=0,n=o.length;e<n;e+=1)o[e].destroy&&r.call(o[e]);f.removeEvents.call(this),this!==(t=f.getDocument.call(this))&&this!==t.documentElement&&this!==t.body&&this!==f.getWindow.call(this)&&i.call(this)},getParent:function(t){var e=this.parentNode;if(t)for(;e&&1===e.nodeType&&!f.match.call(e,t);)e=e.parentNode;return e&&1!==e.nodeType&&(e=null),e?f.extend(e):null},getParents:function(t){for(var e=[],n=this;;){var i=n.getParent(t);if(!i)return e;e.push(i),n=i}},getClosest:function(t){return f.match.call(this,t)?this:f.getParent.call(this,t)},getChildren:function(){return Array.prototype.filter.call(this.childNodes,function(t){return 1===t.nodeType}).map(f.extend)},getDocument:function(){return 9===this.nodeType?this:this.ownerDocument||this.document},getWindow:function(){var t=f.getDocument.call(this);return t&&(t.defaultView||t.parentWindow)},getOffsetParent:function(){var t;function e(){var e=document.createElement("div"),n=document.createElement("div");e.style.height="0",e.appendChild(n),t=n.offsetParent===e}function n(t){return/^(?:body|html)$/i.test(t.tagName)}function i(t){return t&&("static"!==f.getStyle.call(t,"position")||n(t))}function r(t){return i(t)||/^(?:table|td|th)$/i.test(t.tagName)}return function(){var o,a=this,s=f.getDocument.call(a),l=a.offsetParent||s&&s.body,c=f.getStyle.call(a,"position");if(!n(a)&&"fixed"!==c)if(void 0===t&&e(),t){for(o="static"===c?r:i;void 0!==(a=a.parentNode);)if(o(a)){l=a;break}}else try{l=a.offsetParent}catch(t){}return l&&(l=f.extend(l)),l}}(),getElements:function(t){return Array.prototype.map.call(v("querySelectorAll",t,this),f.extend,e)},getElement:function(t){return f.extend(v("querySelector",t,this))},match:function(t,e){return v("matchesSelector",t,e,this)},hasClassName:function(t){var e=O(this);return Boolean(e&&n.contains(e,t," "))},addClassName:function(t){return f.hasClassName.call(this,t)||D(this,(O(this).trim()+" "+t).trim()),this},removeClassName:function(t){return D(this,O(this).replace(new RegExp("(^|\\s)"+t+"(?:\\s|$)"),"$1").trim()),this},toggleClassName:function(t,n){var i=e.is(n)?n:!f.hasClassName.call(this,t);return e.Element[i?"addClassName":"removeClassName"].call(this,t)},setStyle:function(t,e){var n={};return n[t]=e,f.setStyles.call(this,n)},setStyles:function(){var t={},i={none:"",firefox:"-moz-",opera:"-o-",trident:"-ms-",webkit:"-webkit-"},r={columnCount:1,flex:1,flexGrow:1,flexShrink:1,fontWeight:1,lineClamp:1,lineHeight:1,opacity:1,order:1,orphans:1,widows:1,zIndex:1,zoom:1,fillOpacity:1,strokeOpacity:1};function a(t){var e=[];return t.replace(/['"]/g,"").split(",").forEach(function(t){e.push('"'+t.trim()+'"')}),e.join(", ")}function s(n){var r=function(e,n){var r,a,s,l,c=e+n;if(t[c])r=t[c];else{for(a in r=!1,l=document.createElement("div").style,i)if(s=i[a]+n,l[e]=s,l[e]===s&&""!==s&&!o.Engine.ie){r=s;break}t[c]=r}return r}("cursor",n);return n=!1!==r?r:o.Engine.opera?"move":"url("+e.hosts.uwa+e.paths.css+"/base/cursor/"+("grabbing"===n?"closedhand":"openhand")+".cur)"+(o.Engine.ie?"":" 4 4")+", move"}return function(t){var i,o,l,c,d=this.style,h=[];for(c in t)t.hasOwnProperty(c)&&(l=t[c],"opacity"===(c=n.camelCase(c))?f.setOpacity.call(this,l):(""!==l&&null!==l&&isFinite(l)&&void 0===r[c]?l+="px":"none"===l&&"userSelect"===c&&void 0!==d.MozUserSelect?l="-moz-none":"fontFamily"===c?l=a(l):"cursor"===c&&("grabbing"!==l&&"grab"!==l||(l=s(l))),h.push({name:f.getStyleName.call(this,c),value:l})));for(i=0,o=h.length;i<o;i++){c=h[i].name,l=h[i].value;try{d[c]=l||0===l?l:""}catch(t){e.log('Unable to set style "'+c+'" with value "'+l+'"')}}return this}}(),getStyle:function(t,e){return f.getStyles.call(this,[t],e)[t]},getStyles:function(){var t,e,n,i=/^-?(?:\d*\.)?\d+(?!px)[^\d\s]+$/i,r=/^margin/;return document.defaultView&&document.defaultView.getComputedStyle?t=function(t,n,o){var a,s,l,c,d,h,u,m=t.ownerDocument,g=m.defaultView,p=f.getWindow.call(t).getComputedStyle(t,null),v=t.style;if(g&&p)for(a=0,s=n.length;a<s;a++)c=n[a],""!==(d=p[h=f.getStyleName.call(t,c)])&&"auto"!==d||f.isInjected.call(t,m.documentElement)||(d=v[h]),void 0===e&&(u=void 0,(u=document.createElement("div")).style.margin="1%",document.body.appendChild(u),e="1%"===(window.getComputedStyle(u,null)||{marginTop:0}).marginTop,document.body.removeChild(u)),e&&r.test(h)&&i.test(d)&&(l=v.width,v.width=d,d=p.width,v.width=l),o[c]=void 0!==d?d:v[c]||"";return o}:document.documentElement.currentStyle&&(t=function(t,e,n){var r,o,a,s,l,c,d,h=t.currentStyle,u=t.runtimeStyle,m=t.style;for(r=0,o=e.length;r<o;r++)s=e[r],d=f.getStyleName.call(t,s),l=h&&h[d],i.test(l)&&(a=m.left,(c=u&&u.left)&&(u.left=h.left),m.left="fontSize"===d?"1em":l||0,l=m.pixelLeft+"px",m.left=a,c&&(u.left=c)),n[s]=void 0!==l?l:t.style[s]||"";return n}),function(e,i){var r={};return-1===e.indexOf("opacity")||n||(n=!0,r.opacity=f.getOpacity.call(this,i),e.splice(e.indexOf("opacity"),1),n=!1),r=!1===i?function(t,e,n){var i,r,o,a=t.style;for(i=0,r=e.length;i<r;i++)n[o=e[i]]=a[o]||"";return n}(this,e,r):t(this,e,r)}}(),getStyleName:function(){var t=o.Engine,e=t.name,i=["box-sizing","box-shadow","transform","transform-style","transition","transition-timing-function","transition-duration","transition-delay","transition-property","border-image","border-radius","text-stroke","font-smoothing","text-fillcolor","text-shadow","perspective","appearance","touch-callout","overflow-scrolling","mask","user-select"];return r.memoize(function(r,o){var a,s,l=[],c={firefox:"-moz",opera:"-o",ie:o?"-ms":"ms",chrome:"-webkit",safari:"-webkit"};if("string"==typeof r){if("float"===(r=n.unCamelCase(r)))a=t.ie?"style-float":"css-float";else if(-1!==i.indexOf(r)){if(c[e])a=c[e]+"-"+r,l.push(a);else for(s in c)c.hasOwnProperty(s)&&(a=c[s]+"-"+r,-1===l.indexOf(a)&&l.push(a));a=0===(l=l.filter(function(t){return void 0!==u.style[n.camelCase(t)]})).length?r:l.shift()}else a=r;o||(a=n.camelCase(a))}else a=r;return a},function(t){return t.join(".")})}(),getOpacity:(E=function(){},C=o.Features.opacityCSS,S=o.Features.filterCSS,T=/alpha\(opacity=([\d.]+)\)/i,S&&!C?E=function(t,e){var n,i=1;return(n=f.getStyle.call(t,"filter",e).replace(/ /g,"").match(T))&&(i=n[1]/100),i}:C&&(E=function(t,e){var n=1,i=t.style,r=f.getStyle;return void 0!==i.opacity?n=r.call(t,"opacity",e):void 0!==i.MozOpacity&&(n=r.call(t,"MozOpacity",e)),parseFloat(Math.round(100*n)/100,10)}),function(t){return E(this,t)}),setOpacity:function(){var t=function(){},e=o.Features.opacityCSS;return o.Features.filterCSS&&!e?t=function(t,e,n){var i;e.zoom=1,n=1===n?"":"alpha(opacity="+100*n+")",e.MsFilter=n,e.filter=n,i=e.display,e.display="none",t.offsetHeight,e.display=i}:e&&(t=function(t,e,n){void 0!==e.opacity?e.opacity=n:void 0!==e.MozOpacity&&(e.MozOpacity=n)}),function(e){var n=this.style;return null!==e&&(e=(e=parseFloat(e,10))>1?1:e<1e-5?0:e),t(this,n,e),this}}(),hide:function(){return f.setStyle.call(this,"display","none")},show:function(){var t,e,n;function i(t){return f.getStyle.call(t,"display")}return n=r.memoize(function(n){var r,o=document,a=o.body,s=o.createElement(n);return a.appendChild(s),r=i(s),a.removeChild(s),"none"!==r&&""!==r||(t||((t=o.createElement("iframe")).frameBorder=t.width=t.height=0),a.appendChild(t),e&&t.createElement||((e=(t.contentWindow||t.contentDocument).document).write(("CSS1Compat"===o.compatMode?"<!doctype html>":"")+"<html><body>"),e.close()),s=e.createElement(n),e.body.appendChild(s),r=i(s),a.removeChild(t)),r}),function(){var t;return this.style&&("none"===(t=this.style.display)&&(t=this.style.display=""),""===t&&(this.style.display="none"===i(this)&&n(this.nodeName)||"")),this}}(),toggle:function(t){var n=e.is(t)?t:f.isHidden.call(this);return e.Element[n?"show":"hide"].call(this)},isHidden:function(){return"none"===f.getStyle.call(this,"display")},setTranslate:(x=o.Features.transitionsCSS?o.Features.matrixCSS?function(t,e){return{transform:"translate3d("+e+"px,"+t+"px, 0)"}}:function(t,e){return{transform:"translate("+e+"px,"+t+"px)"}}:function(t,e){return{top:t,left:e}},function(t,e){var n;return n=x(t=t||0,e=e||0),f.setStyles.call(this,n),this}),getComputedSize:(b={borderWidth:["borderLeftWidth","borderRightWidth"],borderHeight:["borderBottomWidth","borderTopWidth"],paddingWidth:["paddingLeft","paddingRight"],paddingHeight:["paddingTop","paddingBottom"],marginWidth:["marginLeft","marginRight"],marginHeight:["marginTop","marginBottom"],innerWidth:["borderWidth","paddingWidth"],innerHeight:["borderHeight","paddingHeight"],outerWidth:["marginWidth"],outerHeight:["marginHeight"]},function(){var t,e,i,o,a=r.toArray(arguments),s=0;for(t=0;t<a.length;t++)i=n.camelCase(a[t]),b[i]?(a.splice(t,1),a=a.concat(b[i]),t--):a.splice(t,1,i);for(o=f.getStyles.call(this,a),t=0,e=a.length;t<e;t++)i=a[t],s+=parseFloat(o[i],10)||0;return s}),getScrolls:function(){var t;return function(){var n,i,r,a,s;return e.is(this,["window","document"])?i=o.getScrolls():(r=this.style,i={width:this.scrollWidth,height:this.scrollHeight,top:this.scrollTop,left:this.scrollLeft},void 0===t&&(a=document.createElement("div"),(s=document.createElement("div")).style.visibility="hidden",s.style.overflow="hidden",s.style.width="1px",a.style.overflow="visible",a.innerHTML="x",s.appendChild(a),u.appendChild(s),t=1===a.scrollWidth,u.removeChild(s)),t&&-1!==["","visible"].indexOf(f.getStyle.call(this,"overflow"))&&(n=r.overflow,r.overflow="hidden",i.width=this.scrollWidth,r.overflow=n)),i}}(),getOffsets:function(){var t,e,n,i,r,a=/^t(?:able|d|h)$/i;function s(t){var e=t.ownerDocument.defaultView;return e?e.getComputedStyle(t,null):t.currentStyle}function l(t,e){return f.getStyle.call(t,e)}function c(){var o,a,s,c=document.body,d=parseInt(l(c,"marginTop"),10),h=document.createElement("div");h.innerHTML="<div style='position:absolute;top:0;left:0;margin:0;border:5px solid #000;padding:0;width:1px;height:1px;'><div></div></div><table style='position:absolute;top:0;left:0;margin:0;border:5px solid #000;padding:0;width:1px;height:1px;' cellpadding='0' cellspacing='0'><tr><td></td></tr></table>",c.insertBefore(h,c.firstChild),a=(o=h.firstChild).firstChild,s=o.nextSibling.firstChild.firstChild,t=5!==a.offsetTop,e=5===s.offsetTop,a.style.position="fixed",a.style.top="20px",n=20===a.offsetTop||15===a.offsetTop,a.style.position=a.style.top="",o.style.overflow="hidden",o.style.position="relative",i=-5===a.offsetTop,r=c.offsetTop!==d,c.removeChild(h)}function d(e){var n=e.offsetTop,i=e.offsetLeft;return void 0===t&&c(),r&&(n+=parseFloat(l(e,"marginTop"))||0,i+=parseFloat(l(e,"marginLeft"))||0),{x:i,y:n}}return void 0!==document.documentElement.getBoundingClientRect?function(){if(this===this.ownerDocument.body)return d(this);var t,e,n,i,r,a,s,l=f.getWindow.call(this),c=l.webkitConvertPointFromNodeToPage;if(this.getBoundingClientRect){i=f.getDocument.call(this).body,r=u.clientTop||i.clientTop||0,a=u.clientLeft||i.clientLeft||0,s=o.getScrolls();try{n=this.getBoundingClientRect()}catch(t){}n&&f.isInjected.call(this,u)?(t=n.left+s.x-r,e=n.top+s.y-a):(t=n?n.left:0,e=n?n.top:0)}else c&&(t=(n=c(this,new l.WebKitPoint(0,0))).x,e=n.y);return{x:t,y:e}}:function(){if(this===this.ownerDocument.body)return d(this);var r,o=this,l=o.offsetParent,h=f.getDocument.call(o).body,m=s(o),g=o.offsetTop,p=o.offsetLeft;for(void 0===t&&c(),o=o.parentNode;o&&o!==h&&o!==u&&11!==o.nodeType&&(!n||"fixed"!==m.position);)r=s(o),p-=o.scrollLeft,g-=o.scrollTop,o===l&&(p+=o.offsetLeft,g+=o.offsetTop,!t||e&&a.test(o.nodeName)||(p+=parseFloat(r.borderLeftWidth)||0,g+=parseFloat(r.borderTopWidth)||0),l=o.offsetParent),i&&"visible"!==r.overflow&&(p+=parseFloat(r.borderLeftWidth)||0,g+=parseFloat(r.borderTopWidth)||0),m=r,o=o.parentNode;return"relative"!==m.position&&"static"!==m.position||(p+=h.offsetLeft,g+=h.offsetTop),n&&"fixed"===m.position&&(p+=Math.max(u.scrollLeft,h.scrollLeft),g+=Math.max(u.scrollTop,h.scrollTop)),{x:p,y:g}}}(),getPosition:function(t,n){var i,r,o,a,s,l,c,d=f.getOffsetParent,h=f.getOffsets,u=f.getComputedSize,m=f.getSize,g=f.isInjected,p={x:0,y:0};if(!(t=t||d.call(this))||!g.call(this))return p;if(c=h.call(this),t!==f.getDocument.call(this)&&(i=/^(?:body|html)$/i.test(t.nodeName)?p:h.call(t),c.x-=parseFloat(u.call(this,"marginLeft"))||0,c.y-=parseFloat(u.call(this,"marginTop"))||0,i.x+=parseFloat(u.call(t,"borderLeftWidth"))||0,i.y+=parseFloat(u.call(t,"borderTopWidth"))||0,c.x-=i.x,c.y-=i.y,l=e.typeOf(n)))for("string"===l&&(n={x:n,y:n}),r=m.call(this),o=0;o<2;o+=1)s=o?"width":"height","center"===n[a=o?"x":"y"]?c[a]+=r[s]/2:(1===o&&"right"===n[a]||0===o&&"bottom"===n[a])&&(c[a]+=r[s]);return c},setPosition:function(){var t={full:function(t,e){var n=f.getSize.call(this),i=t.x+t.width-e.x-n.width,r=t.y+t.height-e.y-n.height;i<0&&(e.x=Math.max(0,e.x+i)),r<0&&(e.y+=r)},"resize-max":function(t,e){f.setStyles.call(this,{maxWidth:t.x+t.width-e.x,maxHeight:t.y+t.height-e.y})},none:function(){}};return function(n,i){i=i||{};var a,s,l=f.getDocument.call(this).body,c=f.getOffsetParent.call(this)||l,d=f.getOffsets.call(c),h=f.getOffsets.call(i.relative||c);return a=function(t,n,i,r,a){var s,l;switch(e.typeOf(r)){case!1:break;case"object":l={x:r.x+i.x,y:r.y+i.y,width:r.width,height:r.height};break;case"element":s=r;break;default:for(s=f.getOffsetParent.call(t);s&&s!==n&&1===s.nodeType&&"visible"===f.getStyle.call(s,"overflow");)s=s.parentNode;s&&1===s.nodeType||(s=n)}return s&&(s===n?l=e.merge(o.getScrolls(),o.getSize()):((l=f.getOffsets.call(s)).width=s.offsetWidth,l.height=s.offsetHeight)),l&&(l.x+=a,l.y+=a,l.width-=2*a,l.height-=2*a),l}(this,l,h,i.boundary,i.boundaryMargin||0),"number"==typeof n.length&&(s=f.getSize.call(this),r.splat(n).forEach(function(t){var e=h.x+t.x,n=h.y+t.y;t.score=(Math.min(a.x+a.width,e+s.width)-Math.max(a.x,e))*(Math.min(a.y+a.height,n+s.height)-Math.max(a.y,n))}),n.sort(function(t,e){return e.score-t.score}),n=n[0]),n={x:n.x+h.x,y:n.y+h.y},a&&(i.fit?"string"==typeof i.fit&&e.owns(t,i.fit)&&(i.fit=t[i.fit]):i.fit=t.full,n.x=Math.max(a.x,Math.min(n.x,a.x+a.width)),n.y=Math.max(a.y,Math.min(n.y,a.y+a.height)),i.fit.call(this,a,n)),f.setStyles.call(this,{top:n.y-d.y,left:n.x-d.x}),this}}(),getSize:function(){var t,n,i,r,a,s,l;return e.is(this,["window","document"])?l=o.getSize():(s=f.getStyle.bind(this),i=this.style,r=this.offsetWidth,a=this.offsetHeight,"none"===s("display")&&0===r&&0===a&&(n=i.display,t=i.visibility,i.visibility="visible",i.display="block",r=this.offsetWidth,a=this.offsetHeight,i.display=n,i.visibility=t),l={width:r,height:a}),l},getDimensions:function(){var t,e=f.getSize.call(this),n=e.width,i=e.height,r=f.getStyles.call(this,["maxWidth","maxHeight","minWidth","minHeight","borderLeftWidth","borderRightWidth","paddingLeft","paddingRight","borderBottomWidth","borderTopWidth","paddingTop","paddingBottom","marginLeft","marginRight","marginTop","marginBottom"]);for(t in r)r[t]=parseFloat(r[t],10)||0;return{width:n,height:i,maxWidth:r.maxWidth||-1,maxHeight:r.maxHeight||-1,minWidth:r.minWidth||-1,minHeight:r.minHeight||-1,innerWidth:n-(r.borderLeftWidth+r.borderRightWidth+r.paddingLeft+r.paddingRight),innerHeight:i-(r.borderBottomWidth+r.borderTopWidth+r.paddingTop+r.paddingBottom),outerWidth:n+r.marginLeft+r.marginRight,outerHeight:i+r.marginTop+r.marginBottom}},isInViewport:function(t,e,n,i){var r,a,s,l,c,d,h=f.getOffsets,u=h.call(t),m=h.call(this),g=t.offsetHeight,p=t.offsetWidth,v=this.offsetWidth,y=this.offsetHeight,w=m.y,b=m.x,x=w+this.offsetHeight,E=b+this.offsetWidth;return e?(l=b<u.x+p&&b+v>u.x,c=w<u.y+g&&w+y>u.y):(l=b>=u.x&&b+v<=u.x+p,c=w>=u.y&&w+y<=u.y+g),d="x"===i?l:"y"===i?c:l&&c,n&&(r=o.getScrolls(),a=o.getSize(),s={top:r.y,bottom:r.y+a.height,right:r.x+a.width,left:r.x},d=d&&w<s.bottom&&b<s.right&&x>s.top&&E>s.left),d},setData:function(t,i){var r,o=e.typeOf(i),a=e.typeOf(t);if("string"===a&&o)i=s.encode(i),this.dataset?this.dataset[n.camelCase(t)]=i:(t="data-"+n.unCamelCase(t),this.setAttribute?this.setAttribute(t,i):this[t]=i);else if("object"===a&&!o)for(r in t)t.hasOwnProperty(r)&&f.setData.call(this,r,t[r]);return this},getData:function(t){var i;return e.is(t,"string")&&(this.dataset?i=this.dataset[n.camelCase(t)]:(t="data-"+n.unCamelCase(t),i=this.getAttribute?this.getAttribute(t,i):this[t]=i)),e.is(i)?s.decode(i):void 0},removeData:function(t){return e.is(t,"string")&&(this.dataset?this.dataset.hasOwnProperty(n.camelCase(t))&&delete this.dataset[n.camelCase(t)]:(t="data-"+n.unCamelCase(t),this.removeAttribute?this.removeAttribute(t):this[t]=null)),this},handleExternalLinks:function(t){return f.addEvent.call(this,"click",function(e){if(!l.isDefaultPrevented(e)&&!l.whichKey(e)){for(var n,i=l.getElement(e),r=String(window.location).split("#")[0];i&&!n;)n="a"===f.getTagName.call(i)&&i.getAttribute("href")||f.getData.call(i,"href"),i=f.getParent.call(i);n&&0!==n.indexOf(r+"#")&&0!==n.indexOf("#")&&0!==n.indexOf("javascript")&&(t(n),l.stop(e))}}),this},addEvent:function(){return function(t,n,i,r,o){t=y(t);var a=n&&"function"==typeof n.handleEvent?n:this,s=function(t,n,i,r){e.is(t,"window")&&"resize"===n&&(i=!0);var o,a,s=t._events||{},l=!i&&f.Events[n],c=l?n+"Custom":n,h=s[c];return h||(a=new L(t),s[c]=h={dispatcher:a,handleEvent:function(t){if(d){var n=window.DOMEvent||window.Event;t=new n(t),["offsetY","offsetX","relatedTarget","button","metaKey","altKey","shiftKey","ctrlKey","clientY","clientX","screenY","screenX","which","pageY","pageX","layerY","layerX","charCode","keyCode","timeStamp","cancelable","bubbles","target","type","detail","wheelDelta","touches","changedTouches"].forEach(function(n){e.owns(t,n)||(t[n]=t.event[n])})}void 0===t.timeStamp&&(t.timeStamp=Date.now()),a.dispatch([t])},events:{},bindings:[],timers:[]},o=h.handleEvent,t._events=s,l?l(h,t,{target:t,type:n}):t.addEventListener?t.addEventListener(n,o,r||!1):(t.attachEvent("on"+n,o),window.attachEvent("onunload",function(){t.detachEvent("on"+n,o)}))),h}(this,t.name,i,o);return s.dispatcher.addDelegation(n,t.selector,a,r),"load"===t.name&&this.tagName&&"img"===this.tagName.toLowerCase()&&this.complete&&this.width>0&&s.dispatcher.dispatch(),this}}(),addEvents:function(t,e,n,i){var r;for(r in t)t.hasOwnProperty(r)&&f.addEvent.call(this,r,t[r],e,n,i);return this},triggerEvent:function(t){var e=(this._events||{})[t],n={target:this,timeStamp:Date.now(),type:t};return e&&e.handleEvent(n),this},removeEvent:function(t,n,i){if(!e.is(t))return f.removeEvents.call(this);t=y(t);var r,o,a,s,l,c=this._events&&this._events[t.name+"Custom"],d=c?t.name+"Custom":t.name,h=this._events&&this._events[d];if(h&&(s=h.dispatcher,n||t.selector?s.removeDelegation(n,t.selector):s.removeAll(),0===s.getNumListeners())){for(a in delete this._events[d],l=h.events)l.hasOwnProperty(a)&&f.removeEvent.call(this,a,l[a]);if(h.timers)for(r=0,o=h.timers.length;r<o;r++)clearTimeout(h.timers[r]);if(h.bindings)for(r=0,o=h.bindings.length;r<o;r++)h.bindings[r].dispose();c||(this.removeEventListener?this.removeEventListener(d,h.handleEvent,i):this.detachEvent("on"+d,h.handleEvent)),s.dispose()}return this},removeEvents:function(t,e){var n,i=void 0!==t,r=i?t:this._events;for(n in r)r.hasOwnProperty(n)&&f.removeEvent.call(this,n,i?t[n]:null,e);return this},fillParent:function(t,e){t=t||"height";var i=e||f.getParent.call(this),r=f.setStyle.bind(this),o=n.ucfirst(t);return i&&(r("height",1e4+"px"),r("height",i["offset"+o]-i["scroll"+o]+1e4+"px")),this},setSelectable:function(){function t(t){l.preventDefault(t)}return function(e){return this.setAttribute("unselectable",e?"off":"on"),f.setStyles.call(this,{userSelect:e?"":"none",touchCallout:e?"":"none"}),f[e?"removeEvent":"addEvent"].call(this,"selectstart",t),this}}(),requestFullscreen:(w=h(u,"requestFullscreen")||h(u,"requestFullScreen"),w?function(){return w.call(this)}:function(){throw new Error("Element#requestFullscreen is not available in this platform")})}),f.Events={mouseleave:function(){return function(t,e,n){var i=t.handleEvent;e.addEventListener?(t.handleEvent=function(t){var e=t.relatedTarget;this===e||function(t,e){var n=!1;if(t!==e){for(;e&&e!==t;)e=e.parentNode;n=t===e}return n}(this,e)||i.call(this,n)},f.addEvent.call(e,"mouseout",t.handleEvent),t.events.mouseout=t.handleEvent):(f.addEvent.call(e,"mouseleave",i,!0),t.events.onmouseleave=i)}}(),mouseenter:function(){return function(t,e,n){var i=t.handleEvent;e.addEventListener?(t.handleEvent=function(t){var e=t.relatedTarget;this===e||function(t,e){var n=!1;if(t!==e){for(;e&&e!==t;)e=e.parentNode;n=t===e}return n}(this,e)||i.call(this,n)},f.addEvent.call(e,"mouseover",t.handleEvent),t.events.mouseover=t.handleEvent):(f.addEvent.call(e,"mouseenter",i,!0),t.events.mouseenter=i)}}(),mousewheel:function(t,e){var n=t.handleEvent,i=o.Engine.firefox?"DOMMouseScroll":"mousewheel";t.handleEvent=function(t){(t=t||window.event).wheel=t.wheelDelta?t.wheelDelta/120:-(t.detail||0)/3,n(t)},f.addEvent.call(e,i,t.handleEvent,!0),t.events[i]=t.handleEvent},update:function(t,e,n){new c(function(e){var i=e[0];t.handleEvent(Object.assign(n,{record:i}))}).observe(e,{childList:!0,subtree:!0})},resize:function(){var t,n=new a,i=200;function r(t){var n;return(n=e.is(t,["window","document"])?[(n=o.getSize()).width,n.height,0,0]:[t.scrollWidth,t.scrollHeight,t.offsetWidth,t.offsetHeight]).join("x")}function s(){clearTimeout(t),n.dispatch(),n.getNumListeners()>0&&(t=setTimeout(s,i))}return function(t,i,o){var a,l=r(i);t.bindings.length>0||(t.timers=[a],window===i&&e.is(window.orientationchange)&&(f.addEvent.call(i,"orientationchange",s),t.events.orientationchange=s),t.bindings=[n.add(function(){var n=r(i),s=e.is(i,["window","document"])||f.isInjected.call(i);l!==n&&s&&(l=n,clearTimeout(a),a=setTimeout(function(){t.handleEvent(o)},220))})],s())}}()},N("fullscreenchange"),N("fullscreenerror"),N("transitionEnd",function(){var t,n=document.createElement("fakeelement"),i={WebkitTransition:"webkitTransitionEnd",MozTransition:"transitionend",msTransition:"MSTransitionEnd",OTransition:"oTransitionEnd",transition:"transitionEnd"};for(t in i)if(i.hasOwnProperty(t)&&e.is(n.style[t]))return i[t]}),u.matchesSelector||(f.matchesSelector=h(u,"matchesSelector")),document.exitFullscreen=h(document,"exitFullscreen")||h(document,"cancelFullScreen")||function(){throw new Error("Element#requestFullscreen is not available in this platform")},"fullscreenEnabled"in document||(document.fullscreenEnabled=h(document,"fullscreenEnabled")),function(){var t="fullscreenElement",e=h(document,t,!0)||h(document,"fullScreenElement",!0)||h(document,"currentFullScreenElement",!0);if(e&&e!==t)try{f.addEvent.call(document,"fullscreenchange",function(){document[t]=document[e]}),document[t]=document[e]}catch(t){}}(),H(),l.onDomReady(H),e.namespace("Element",f,e,!0)});
define("UWA/Internal/StringMap",["UWA/Class"],function(t){"use strict";function n(t){return"_x_"+t}return t.extend({init:function(){this._data={}},get:function(t){return this._data[n(t)]},set:function(t,i){return this._data[n(t)]=i,this},getAll:function(){var t={};for(var n in this._data)t[n.slice(3)]=this._data[n];return t},remove:function(t){return delete this._data[n(t)],this}})});
define("UWA/Class/Events",["UWA/Core","UWA/Class","UWA/Dispatcher","UWA/Utils"],function(t,n,e,s){"use strict";var i;function r(t,n,s){var i=t._dispatchers,r=i&&i[n]||new e;return s||(i||(i=t._dispatchers=Object.create(null)),i[n]=r),r}return i=n.extend({dispatchEvent:function(t,n,e){var i,a;return void 0===e&&(e=this),n=s.splat(n),i=r(this,t),"function"==typeof this[t]&&i.addOnce(this[t],e,1),"onAnyEvent"!==t&&this.hasEvent("onAnyEvent")?(a=r(this,"onAnyEvent"),"function"==typeof this.onAnyEvent&&a.addOnce(this.onAnyEvent,e),a.addOnce(function(){i.dispatch(n,e)}),a.dispatch([t].concat(n),e)):i.dispatch(n,e),this},dispatchAsEventListener:function(t,n,e){var i=this;return void 0===e&&(e=i),n=s.splat(n),function(s){i.dispatchEvent(t,[s].concat(n),e)}},addEvent:function(t,n,e,s){return r(this,t).add(n,e,s),this},addEventOnce:function(t,n,e,s){return r(this,t).addOnce(n,e,s),this},addEvents:function(t,n,e){var s;for(s in t)t.hasOwnProperty(s)&&this.addEvent(s,t[s],n,e);return this},removeEvent:function(t,n,e){var s,i=this._dispatchers,r=i&&i[t];if(t)r&&(n?r.remove(n,e):r.removeAll(e),0===r.getNumListeners()&&delete i[t]);else for(s in i)this.removeEvent(s,n,e);return this},removeEvents:function(t){var n;if(t)for(n in t)t.hasOwnProperty(n)&&this.removeEvent(n,t[n]);else this.removeEvent();return this},hasEvent:function(t,n){var e,s=this;return e=function(t){return!!(r(s,t,!0).getNumListeners()||!n&&s[t])},(t?[t]:Object.keys(s._dispatchers||{})).some(e)}}),t.namespace("Events",i,n)});
define("UWA/Data",["UWA/Core","UWA/Utils","UWA/Utils/Client","UWA/Ajax","UWA/Json","UWA/Internal/StringMap","UWA/Class/Events"],function(e,t,r,n,o,a,s){"use strict";var u,i,d=new a,c={proxies:(u=e.hosts,i=u.exposition+"/proxy/",e.merge(u.proxies||{},{ajax:i+"ajax",resolve:i+"resolve",xml:i+"xml",spreadsheet:i+"spreadsheet",soap:i+"soap",feed:i+"feed",icon:i+"icon",richIcon:i+"richIcon",rss:i+"feed"})),useJsonpRequest:!0,allowCrossOriginRequest:!1,useOfflineCache:!1,request:function(){var a=/OPTIONS|GET|HEAD|POST|PUT|DELETE|TRACE|CONNECT/i,u=/json|document|blob|arraybuffer|text/,i=/^([A-Za-z0-9+/]{4})*([A-Za-z0-9+/]{4}|[A-Za-z0-9+/]{3}=|[A-Za-z0-9+/]{2}==)$/,d=r.isOnline;var p={text:function(e){return"string"!=typeof e&&(e=o.encode(e)),e},json:function(t){if("string"==typeof t&&(t=o.decode(t)),!e.is(t,["object","array"]))throw new Error('Invalid JSON Response: "'+String(t)+'"');return t},xml:function(e){return"string"==typeof e&&(e=t.loadXml(e)),e},document:function(e){return"string"==typeof e&&(e=t.loadHtml(e)),e},blob:function(e,r){var n=t.getOwnPropertyMatchValue(r,"Content-Type")||"text/plain";return"string"==typeof e&&(e=i.test(e)?function(e,t){var r,n,o=e.indexOf(";base64,")+";base64,".length,a=e.substring(o),s=window.atob(a),u=s.length,i=new Uint8Array(u);for(r=0;r<u;++r)i[r]=s.charCodeAt(r);return(n=new BlobBuilder).append(i.buffer),n.getBlob(t)}(e,n):new Blob([e],{type:n})),e},arraybuffer:function(e){return"string"==typeof e&&(e=new ArrayBuffer(12)),e}};return function(r,h){if(!r)throw new Error("Bad or missing url argument.");h=h||{};var l,f,m,y,g,C,x,w,q,O,T,E,v=window.location,U={timeout:25e3,method:"GET",type:"text",proxy:!1,async:!0,headers:{},useMergeRequest:!0,useOfflineCache:c.useOfflineCache,allowCrossOriginRequest:c.allowCrossOriginRequest,useJsonpRequest:c.useJsonpRequest,onComplete:function(){},onCancel:function(){},onFailure:function(e){throw e}};return h.requestHeaders&&(h.headers=h.requestHeaders,delete h.requestHeaders),h.postBody?(h.method="POST",h.data=h.postBody,delete h.postBody):h.parameters&&(h.method="POST",h.data=h.parameters,delete h.parameters),h.auth&&(h.authentication=h.auth,delete h.auth),"html"===h.type?h.type="document":"feed"===h.type&&(h.type="json"),(h=e.merge(h,U)).type=p[h.type]?h.type:U.type,h.timeout=parseInt(h.timeout,10),a.test(h.method)&&(h.method=h.method.toUpperCase()),"json"===h.type&&(t.getOwnPropertyMatchName(h.headers,"Accept")||(h.headers.Accept="application/json,text/javascript,*/*"),t.getOwnPropertyMatchName(h.headers,"X-Request")||(h.headers["X-Request"]="JSON")),w=h.type,q=h.useOfflineCache,O=h.allowCrossOriginRequest,T=h.useJsonpRequest,E=r,h.proxy?(r=c.proxifyUrl(r,h),T=T&&!1===t.matchUrl(r,v)&&!1===O):!1===t.matchUrl(r,v)&&!1===O?(T=T&&!1===t.matchUrl(c.proxies.ajax,v),r=c.proxifyUrl(r,e.extend(h,{proxy:"ajax"}))):T=!1,c.requests=c.requests||{},g=function(r,n){var o={url:r,timeout:n.timeout,method:n.method,type:n.type,proxy:n.proxy,async:n.async,data:n.data,headers:n.headers};return"GET"===n.method&&!1!==n.useMergeRequest||(o.uuid=t.getUUID()),e.Json.encode(o)}(r,h),f={onComplete:h.onComplete,onFailure:h.onFailure,onCancel:h.onCancel,onTimeout:h.onTimeout||h.onFailure},c.requests[g]?(l=c.requests[g]).addEvents(f):((l=c.requests[g]=new s).addEvents(f),C=function(e,r){var n=e;delete c.requests[g],t.attempt(function(){var o;return T&&(r=e.headers,o=e.body,i.test(o)&&(o=t.base64Decode(o)),e=o),e=p[w](e,r),q&&c.storeInCache(E,n),!0},function(){return x("onFailure",arguments),!1})&&l.dispatchEvent("onComplete",[e,r])},x=function(t,r){var n,o,a=!0;delete c.requests[g],q&&(n=c.getFromCache(E),e.is(n)&&(a=!1,d()&&d(!1,o||5e3),C(n))),a&&l.dispatchEvent(t,r)},m={method:h.method,data:h.data,headers:h.headers,fromDataRequest:E,timeout:h.timeout,async:h.async,withCredentials:h.withCredentials,onComplete:function(e,t){C(e,t)},onFailure:function(){x("onFailure",arguments)},onCancel:function(){x("onCancel",arguments)},onTimeout:function(){x("onTimeout",arguments)},onProgress:h.onProgress},q&&!1===d()?m.onFailure(new Error("Network is Offline")):T?(h.data&&h.data.length>0&&-1!==["POST","PUT"].indexOf(h.method)&&(r+=-1!==r.indexOf("?")?"&":"?","POST"===h.method?r+=t.toQueryString(h.data,"postData"):"PUT"===h.method&&(r+=t.toQueryString(h.data,"rawData")),delete m.data,delete m.method),y=o.request(r,m)):(w&&u.test(w)&&(m.responseType=w),l.xhr=y=n.request(r,m)),l.url=E,l.options=h,l.cancel=y.cancel),l}}(),proxifyUrl:function(e,r){if(!e)throw new Error("Bad or missing url argument.");var n,o=[],a=r.proxy,s=t.toQueryString,u=c.proxies;if(!a||!u[a])throw new Error("Invalid proxy");if(n=u[a],0===e.indexOf(n))return e;if(r.data&&r.method&&"GET"===r.method.toUpperCase()&&(e+=(e.indexOf("?")>-1?"&":"?")+s(r.data),delete r.data),"object"==typeof r[a]&&(o.push(s(r[a])),delete r[a]),r.type&&(o.push(s({type:r.type})),delete r.type),"object"==typeof r.authentication&&o.push(s(r.authentication)),r.cache&&(o.push(s({cache:parseInt(r.cache,10)})),r.cache<0&&o.push(Date.now())),r.headers&&(o.push(s(r.headers,"headers")),delete r.headers),r.connect&&o.push(s({connect:r.connect})),r.service&&o.push(s({service:r.service})),r.wid&&o.push(s({wid:r.wid})),r.method&&o.push(s({method:r.method})),o.push(s({url:e})),(e=n+"?"+o.join("&")).length>2048)throw new Error("Proxified url is more than 2048 characters, that is the limit for most of the browsers.");return e},getFeed:function(e,t){return c.request(e,{method:"GET",proxy:"feed",type:"json",onComplete:t})},getXml:function(e,t){return c.request(e,{method:"GET",type:"xml",onComplete:t})},getText:function(e,t){return c.request(e,{method:"GET",type:"text",onComplete:t})},getJson:function(e,t){return c.request(e,{method:"GET",type:"json",onComplete:t})},getCache:function(){return d},storeInCache:function(r,n){n=t.toArray(n).filter(function(t){return e.is(t)&&!t.nodeType}),c.getCache().set(t.getCheckSum(r),n)},getFromCache:function(e){return c.getCache().get(t.getCheckSum(e))}};return e.namespace("Data",c,e)});
define("UWA/Utils/Cookie",["UWA/Core"],function(e){"use strict";var t={},n=window.document,o="nv.",r=new Date("Fri, 31 Dec 9999 23:59:59 UTC"),i=null,a=null;function c(e,t){if(t=t||new Date,"number"==typeof e?e=e===1/0?r:new Date(t.getTime()+1e3*e):"string"==typeof e&&(e=new Date(e)),e&&(n=e,"[object Date]"!==Object.prototype.toString.call(n)||isNaN(n.getTime())))throw new Error("`expires` parameter cannot be converted to a valid Date instance");var n;return e}function u(e){var t=e.indexOf("=");t=t<0?e.length:t;var n,o=e.substr(0,t);try{n=decodeURIComponent(o)}catch(e){throw new Error('Could not decode cookie with key "'+o+'" ['+e+"]")}return{key:n,value:e.substr(t+1)}}function s(){i=function(e){for(var t={},n=e?e.split("; "):[],r=0;r<n.length;r++){var i=u(n[r]);void 0===t[o+i.key]&&(t[o+i.key]=i.value)}return t}(n.cookie),a=n.cookie}return t.defaults={path:"/",secure:!1},t.get=function(e){a!==n.cookie&&s();var t=i[o+e];return void 0===t?void 0:decodeURIComponent(t)},t.getAll=function(){a!==n.cookie&&s();var e={};for(var t in i)e[t.slice(o.length)]=decodeURIComponent(i[t]);return e},t.set=function(e,o,r){return(r=function(e){return{path:e&&e.path||t.defaults.path,domain:e&&e.domain||t.defaults.domain,expires:e&&e.expires||t.defaults.expires,secure:e&&void 0!==e.secure?e.secure:t.defaults.secure}}(r)).expires=c(void 0===o?-1:r.expires),n.cookie=function(e,t,n){var o=(e=(e=e.replace(/[^#$&+\^`|]/g,encodeURIComponent)).replace(/\(/g,"%28").replace(/\)/g,"%29"))+"="+(t=String(t).replace(/[^!#$&-+\--:<-\[\]-~]/g,encodeURIComponent));return o+=(n=n||{}).path?";path="+n.path:"",o+=n.domain?";domain="+n.domain:"",o+=n.expires?";expires="+n.expires.toUTCString():"",o+=n.secure?";secure":""}(e,o,r),t},t.expire=function(e,n){return t.set(e,void 0,n)},t.enabled=function(){var e=!1;try{e="1"===t.set("cookie.js",1).get("cookie.js"),t.expire("cookie.js")}catch(e){}return e}(),e.namespace("Utils/Cookie",t,e)});
define("UWA/Class/Options",["UWA/Core","UWA/Class"],function(t,s){"use strict";var n=s.extend({setOptions:function(s){return s=s||{},this.hasOwnProperty("options")||(this.options=t.clone(this.defaultOptions||this.options||{})),s.events&&this.addEvents&&this.addEvents(s.events),t.extend(this.options,s,!0),this},setOption:function(t,s){var n={};return n[t]=s,this.setOptions(n)},getOption:function(t,s){var n=this.options;return void 0!==n[t]?n[t]:s}});return t.namespace("Options",n,s)});
define("UWA/Class/Debug",["UWA/Core","UWA/Class"],function(e,t){"use strict";var u=t.extend({debugMode:!1,setDebugMode:function(e){return this.debugMode=!0===e||"true"===e,this},log:function(t){return!0===this.debugMode&&e.log(t),this}});return e.namespace("Debug",u,t)});
define("UWA/Storage",["UWA/Internal/Deprecate","UWA/Core","UWA/Class","UWA/Class/Options","UWA/Class/Debug","UWA/Json"],function(e,t,a,r,s,n){"use strict";var i=a.extend(r,s,{AdaptersInstances:null,currentAdapter:null,defaultOptions:{database:"default",adapter:null,adapterOptions:{},availableAdapters:[]},internalKeys:{keysIndex:"_keysIndex",lastUpdate:"_lastUpdate"},isReady:!1,init:function(t){e.warn("UWA/Storage");var a;this.AdaptersInstances={},i.Instances.push(this),this.setOptions(t),(a=this.options.adapter)&&"auto"!==a?this.setCurrentAdapter(a):this.setCurrentAdapterFromDetected()},initAvailableAdapters:function(){var e,t=this,a=t.options.availableAdapters,r=i.Adapter;if(0===a.length)for(e in r)r.hasOwnProperty(e)&&"Abstract"!==e&&a.push(e);a.forEach(function(e){t.getAdapterInstance(e)})},isAvailableAdapter:function(e){var t,a=!1;try{(t=this.getAdapterInstance(e))&&t.isAvailable()?(a=!0,this.log('UWA.Storage:detectAvailableAdapter: "'+e+'" is available')):this.log('UWA.Storage:detectAvailableAdapter: "'+e+'" is not available')}catch(t){this.log('UWA.Storage:detectAvailableAdapter: "'+e+'" is not available cause: '+t)}return a},getAdapterInstance:function(e){var t=this.AdaptersInstances;if("string"!=typeof e)throw new Error('Bad adapterName param value "'+e+'" for getAdapterInstance.');if(!(t[e]||(t[e]=new i.Adapter[e](this,this.options.adapterOptions),t[e]instanceof i.Adapter.Abstract)))throw new Error("UWA.Storage.Adapter."+e+" is not an instance of UWA.Storage.Adapter.Abstract");return t[e]},detectAvailableAdapter:function(){var e=this,t=e.options,a=[];e.initAvailableAdapters(),t.availableAdapters.forEach(function(t){e.isAvailableAdapter(t)&&a.push(t)}),t.availableAdapters=a},setCurrentAdapterFromDetected:function(){var e=this.options;if(this.detectAvailableAdapter(),!(e.availableAdapters.length>0))throw new Error("UWA.Storage: No adapter available detected.");this.setCurrentAdapter(e.availableAdapters[0])},setCurrentAdapter:function(e){var t;if("string"!=typeof e)throw new Error('Bad adapterName param value "'+e+'" for setCurrentAdapter.');this.isAvailableAdapter(e)?((t=this.getAdapterInstance(e)).connect(this.options.database),this.log("UWA.Storage:setCurrentAdapter: "+e+";"),this.adapter=e,this.currentAdapter=t):(this.log('UWA.Storage:setCurrentAdapter: "'+e+'" fail fallback in auto detect mode'),this.setCurrentAdapterFromDetected())},store:function(e,t){var a,r=this.currentAdapter;return r&&(a=this.safeResurrect(r.get(e)),1===arguments.length?this.log('Get Key "'+e+'" with value "'+a+'"'):a!==t&&(a=this.safeStore(t),this.log('Update Key "'+e+'" with value "'+t+'" and stored value "'+a+'"'),a=r.set(e,a))),a},remove:function(e){return!!this.currentAdapter&&(this._updateLastUpdateDate(),this._removeKeyFromKeysIndex(e),this.safeResurrect(this.currentAdapter.rem(e)))},get:function(e,t){var a,r;return t?(a=this._getKeysIndex()).hasOwnProperty(e)&&Date.now()-a[e]<=t&&(r=this.store(e)):r=this.store(e),r},set:function(e,t){return this._updateLastUpdateDate(),this._addKeyToKeysIndex(e),this.store(e,t)},getAll:function(){var e=this,t=Object.keys(this._getKeysIndex()),a={};return t.forEach(function(t){a[t]=e.get(t)}),a},safeStore:function(e){return n.encode(e)},safeResurrect:function(e){if(!t.is(e,"undefined"))try{n.isJson(e)&&(e=n.decode(e))}catch(a){t.log("unsafe Resurrect JSON with value: "+e),t.log(a)}return e},getLastUpdateDate:function(e){var t;return t=e?this._getKeysIndex()[e]:this.get(this.internalKeys.lastUpdate),(new Date).setTime(t)},_getKeysIndex:function(){var e,a,r=this,s=r.safeResurrect(r.currentAdapter.get(this.internalKeys.keysIndex)),n=t.typeOf(s);return r.log("Get all keys from keysIndex"),"array"===n?(e={},a=r.getLastUpdateDate(),s.forEach(function(t){e[t]=a}),s=e):"object"!==n&&(s={}),s},_removeKeyFromKeysIndex:function(e){var t,a=this._getKeysIndex(),r={};for(t in this.log('Remove key "'+e+'" from keysIndex'),a)a.hasOwnProperty(t)&&t!==e&&(r[t]=a[t]);this._storeKeysIndex(r)},_addKeyToKeysIndex:function(e){var t=this._getKeysIndex();this.log('Add key "'+e+'" to keysIndex'),t[e]=Date.now(),this._storeKeysIndex(t)},_storeKeysIndex:function(e){this.currentAdapter.set(this.internalKeys.keysIndex,this.safeStore(e))},_updateLastUpdateDate:function(){var e=Date.now();return this.currentAdapter.set(this.internalKeys.lastUpdate,this.safeStore(e)),e}});return i.Instances=[],t.merge(i,{allInstancesReady:function(){return i.Instances.every(function(e){return e.isReady})}}),t.namespace("Storage",i,t)});
define("UWA/Storage/Adapter/Abstract",["UWA/Core","UWA/Class","UWA/Class/Options","UWA/Storage"],function(t,s,e){"use strict";var r=s.extend(e,{type:"Abstract",limit:-1,init:function(t,s){this.storage=t||{},this.database=null,this.data={},this.includes=[],this.storage.isReady=!1,this.setOptions(s)},isAvailable:function(){return!1},interruptAccess:function(){if(!this.storage.isReady)throw new Error("Storage Adapter "+this.type+" is not ready.");return!0},get:function(t){return this.interruptAccess(),this.data[t]||null},set:function(t,s){return this.interruptAccess(),this.data[t]=s,s},rem:function(t){this.interruptAccess();var s=this.data[t];return this.data[t]=null,s}});return t.namespace("Storage/Adapter/Abstract",r,t)});
define("UWA/Storage/Adapter/Cookies",["UWA/Core","UWA/String","UWA/Utils","UWA/Utils/Cookie","UWA/Storage/Adapter/Abstract"],function(t,e,i,n,s){"use strict";var o=s.extend({type:"Cookies",limit:4096,defaultOptions:{path:"/",duration:100,expires:864e4,secure:!1,domain:""},init:function(t,e){var n=i.parseUrl(window.location);this.defaultOptions={domain:-1!==["80","443"].indexOf(n.port)&&n.domain,secure:"https"===n.protocol},this._parent(t,e),this.options.duration&&(this.options.expires=86400*this.options.duration,delete this.options.duration)},connect:function(t){this.database=t,this.storage.isReady=!0},isAvailable:function(){return n.enabled},getKey:function(t){return"uwa-"+this.database+"-"+t},get:function(t){return this.interruptAccess(),n.get(t)},set:function(t,e){var i=this.options;return this.interruptAccess(),n.set(t,e,i)},rem:function(t){this.interruptAccess();var e=this.options,i=this.get(t);return n.expire(this.getKey(t),e),i}});return t.namespace("Storage/Adapter/Cookies",o,t)});
define("UWA/Function",["UWA/Core"],function(n){"use strict";var t={always:function(n){return function(){return n}}};return n.namespace("Function",t,n)});
define("UWA/Date",["UWA/Core","UWA/Internal/Deprecate"],function(e,t){"use strict";var n={};function r(){t.warn("UWA/Date as a constructor","Use the native Date instead.");var e=Array.prototype.slice.call(arguments);return e.unshift(null),new(Date.bind.apply(Date,e))}return n.strftime=function(){function t(e,t,n){return Array((n||2)-String(e).length+1).join(t||0)+e}function r(e){return parseInt(e,10)}var u=e.i18n,a={a:[u("Sun"),u("Mon"),u("Tue"),u("Wed"),u("Thu"),u("Fri"),u("Sat")],A:[u("Sunday"),u("Monday"),u("Tuesday"),u("Wednesday"),u("Thursday"),u("Friday"),u("Saturday")],b:[u("Jan"),u("Feb"),u("Mar"),u("Apr"),u("May"),u("Jun"),u("Jul"),u("Aug"),u("Sep"),u("Oct"),u("Nov"),u("Dec")],B:[u("January"),u("February"),u("March"),u("April"),u("May"),u("June"),u("July"),u("August"),u("September"),u("October"),u("November"),u("December")],c:u("%a %b %e %Y %T"),p:[u("AM"),u("PM")],P:[u("am"),u("pm")],x:u("%m/%d/%y"),X:u("%T")},o={a:function(e){return a.a[e.getDay()]},A:function(e){return a.A[e.getDay()]},b:function(e){return a.b[e.getMonth()]},B:function(e){return a.B[e.getMonth()]},c:a.c,C:function(e){return t(r(e.getFullYear()/100))},d:function(e){return t(e.getDate())},D:"%m/%d/%y",e:function(e){return t(e.getDate()," ")},F:"%Y-%m-%d",g:function(e){return t(o.G(e)%100)},G:function(e){var t=e.getFullYear(),n=r(o.V(e)),u=r(o.W(e));return u>n?t++:0===u&&n>=52&&t--,t},h:"%b",H:function(e){return t(e.getHours())},I:function(e){return t(e.getHours()%12||12)},j:function(e){return t(r((new Date(e.getFullYear()+"/"+(e.getMonth()+1)+"/"+e.getDate()+" GMT")-new Date(e.getFullYear()+"/1/1 GMT"))/6e4/60/24)+1,0,3)},l:function(e){return t(e.getHours()%12||12," ")},m:function(e){return t(e.getMonth()+1)},M:function(e){return t(e.getMinutes())},n:"\n",p:function(e){return a.p[e.getHours()>=12?1:0]},P:function(e){return a.P[e.getHours()>=12?1:0]},r:"%I:%M:%S %p",R:"%H:%M",s:function(e){return r(e/1e3)},S:function(e){return t(e.getSeconds())},t:"\t",T:"%H:%M:%S",u:function(e){return e.getDay()||7},U:function(e){var n=r(o.j(e));return t(r((n+(6-e.getDay()))/7))},V:function(e){var n=r(o.W(e)),u=new Date(e.getFullYear()+"/1/1").getDay(),a=n+(u>4||u<=1?0:1);return 53===a&&new Date(e.getFullYear()+"/12/31").getDay()<4?a=1:0===a&&(a=o.V(new Date(e.getFullYear()-1+"/12/31"))),t(a,0)},w:function(e){return e.getDay()},W:function(e){var n=r(o.j(e));return t(r((n+(7-o.u(e)))/7))},x:a.x,X:a.X,y:function(e){return t(e.getFullYear()%100)},Y:function(e){return e.getFullYear()},z:function(e,n){var u=n?0:e.getTimezoneOffset();return(u>0?"-":"+")+t(r(Math.abs(u/60)))+t(u%60)},Z:function(e,t){var n;return t?n="UTC":(n=e.toString().replace(/^.*:\d\d( GMT[+\-]\d+)? \(?([A-Za-z ]+)\)?\d*$/,"$2").replace(/[a-z ]/g,"")).length>4&&(n=o.z(e)),n},"%":"%"};return function(e,t,r){var u;return u=r?new Date(Number(e)+6e4*e.getTimezoneOffset()):e,t.replace(/%[A-Za-z%]/g,function(t){var a=o[t.slice(1)];return void 0===a?t:"string"==typeof a?"%"!==a&&a.indexOf("%")>=0?n.strftime(e,a,r):a:a(u,r)})}}(),t.uncurryAlias(n,Date.prototype,"UWA.Date","Date"),["now","parse","UTC"].forEach(function(e){r[e]=t.alias("UWA/Date."+e,"Use the native Date."+e+" instead",Date[e])}),Object.assign(r,n),e.namespace("Date",r,e)});
define("UWA/Object",["UWA/Core","UWA/Internal/Deprecate"],function(e,t){"use strict";function n(){return t.warn("UWA/Object as a constructor","Use the native Object instead."),Object.apply(null,arguments)}return["assign","create","defineProperty","defineProperties","freeze","getOwnPropertyDescriptor","getOwnPropertyNames","getPrototypeOf","isExtensible","isFrozen","isSealed","keys","preventExtensions","seal","setPrototypeOf"].forEach(function(e){n[e]=t.alias("UWA/Object."+e,"Use the native Object."+e+" instead",Object[e])}),e.namespace("Object",n,e)});
define("UWA/Class/Timed",["UWA/Core","UWA/Class","UWA/Utils","UWA/Utils/Client"],function(e,i,t,a){"use strict";var r,n=1,l=a.getVendorProperty(window,"cancelAnimationFrame")||clearTimeout,o=a.getVendorProperty(window,"requestAnimationFrame")||function(e){return setTimeout(e,1e3/60)};function s(e,i,a,r){return function(l,o,s,c,d){var m=this,u=m;return"function"==typeof l&&(d=c,c=s,s=o,o=l,u=l=n++),o=t.attempt.bind(null,o,function(t){throw m[e](l),new Error("The "+i.slice(0,-1)+' "'+l+'" failed with error "'+t+'".')},d||m),m[e](l),m[i]=m[i]||Object.create(null),m[i][l]=a(function(){r&&m[e](l),o()},s),c&&o(),u}}function c(e,i){return function(t){var a,r=this[e];if(r)if(void 0===t)for(a in r)i(r[a]),delete r[a];else r[t]&&(i(r[t]),delete r[t]);return this}}function d(e){return function(i){var t=this[e];return Boolean(t&&t[i])}}return r=i.extend({setPeriodical:s("clearPeriodical","periodicals",window.setInterval),clearPeriodical:c("periodicals",window.clearInterval),hasPeriodical:d("periodicals"),setDelayed:s("clearDelayed","delays",window.setTimeout,!0),clearDelayed:c("delays",window.clearTimeout),hasDelayed:d("delays"),setAnimate:s("clearAnimate","animates",o,!0),clearAnimate:c("animates",l),hasAnimate:d("animates"),setImmediate:s("clearImmediate","immediates",t.setImmediate,!0),clearImmediate:c("immediates",t.clearImmediate),hasImmediate:d("immediates"),clearAllTimed:function(){return this.clearImmediate(),this.clearAnimate(),this.clearDelayed(),this.clearPeriodical(),this}}),e.namespace("Timed",r,i)});
define("UWA/Color",["UWA/Core","UWA/Class"],function(r,a){"use strict";function t(r){return"#"===r.charAt(0)&&(r=r.substring(1)),3===r.length&&(r=r[0]+r[0]+r[1]+r[1]+r[2]+r[2]),{r:parseInt(r.substr(0,2),16),g:parseInt(r.substr(2,2),16),b:parseInt(r.substr(4,2),16)}}function n(a){(a=r.clone(a)).r/=255,a.g/=255,a.b/=255;var t={},n=Math.min(a.r,a.g,a.b),o=Math.max(a.r,a.g,a.b),s=o-n,e=(o+n)/2;return t.l=e,o===n?(t.h=0,t.s=0):(t.h=e,t.s=e,t.s=t.l>.5?s/(2-o-n):s/(o+n),o===a.r?t.h=(a.g-a.b)/s+(a.g<a.b?6:0):o===a.g?t.h=(a.b-a.r)/s+2:o===a.b&&(t.h=(a.r-a.g)/s+4),t.h/=6),t.h=Math.round(360*t.h),t.s=Math.round(100*t.s),t.l=Math.round(100*t.l),t}function o(r){var a={},t=(1-Math.abs(r.l/50-1))*r.s/100,n=t*(1-Math.abs(r.h/60%2-1)),o=Math.floor(r.h/60),s=r.l/100-t/2;switch(o){case 0:a.r=t,a.g=n,a.b=0;break;case 1:a.r=n,a.g=t,a.b=0;break;case 2:a.r=0,a.g=t,a.b=n;break;case 3:a.r=0,a.g=n,a.b=t;break;case 4:a.r=n,a.g=0,a.b=t;break;case 5:case 6:a.r=t,a.g=0,a.b=n}return a.r=Math.round(255*(a.r+s)),a.g=Math.round(255*(a.g+s)),a.b=Math.round(255*(a.b+s)),a}function s(a,t){var n=(a=r.clone(a)).alpha;if(n>=1)return a;return["r","g","b"].forEach(function(r){a[r]=a[r]*n+t[r]*t.alpha*(1-n)}),a.alpha=Math.round(n+t.alpha*(1-n)),a}function e(r){var a=[r.r,r.g,r.b,r.alpha].map(function(r){return(r/=255)<.03928?r/12.92:Math.pow((r+.055)/1.055,2.4)});return.2126*a[0]+.7152*a[1]+.0722*a[2]}function h(r,a){if(a.alpha>=1){r.alpha<1&&(r=s(r,a));var t=e(a)+.05,n=e(r)+.05,o=t/n;return n>t&&(o=1/o),{ratio:Math.round(o),min:o,max:o}}var i={r:255,g:255,b:255,alpha:1},l={r:0,g:0,b:0,alpha:1},u=s(a,l),c=s(a,i),b=h(r,l).ratio,g=h(r,i).ratio,p=Math.max(b,g),f=1;return u.luminance>r.luminance?f=b:c.luminance<r.luminance&&(f=g),{ratio:Math.round((f+p)/2,2),min:f,max:p}}var i=a.extend({_color:null,init:function(a){this._color=r.clone(a)},toHexString:function(){return"#"+[this._color.r,this._color.g,this._color.b].map(function(r){return 1===(r=(r=parseInt(r,10)).toString(16)).length?"0"+r:r}).join("")},toRGBString:function(){var r=this._color,a=r.alpha<1;return"rgb"+(a?"a":"")+"("+r.r+", "+r.g+", "+r.b+(a?", "+r.alpha:"")+")"},toHSLString:function(){var r=this._color,a=r.alpha<1;return"hsl"+(a?"a":"")+"("+r.h+", "+r.s+"%, "+r.l+(a?"%, "+r.alpha:"%")+")"},toObject:function(){return r.clone(this._color)},cloneWith:function(a){var t=Object.assign(this.toObject(),a);return r.owns(a,"h")||r.owns(a,"s")||r.owns(a,"l")?i.fromHSL(t.h,t.s,t.l,t.alpha):r.owns(a,"r")||r.owns(a,"g")||r.owns(a,"b")?i.fromRGB(t.r,t.g,t.b,t.alpha):new i(t)}});return i.fromRGB=function(r,a,t,o){var s={r:parseInt(r,10),g:parseInt(a,10),b:parseInt(t,10),alpha:void 0===o?1:parseFloat(o,10)};return Object.assign(s,n(s)),new i(s)},i.fromHSL=function(r,a,t,n){var s={h:parseInt(r,10),s:parseFloat(a,10),l:parseFloat(t,10),alpha:void 0===n?1:parseFloat(n,10)};return Object.assign(s,o(s)),new i(s)},i.parse=function(r){"transparent"===r&&(r="rgba(0, 0, 0, 0)");var a={},o=r.test(/^(#?)((?:[A-Fa-f0-9]{3}){1,2})$/m),s=r.match(/^(rgb|hsl)(a?)[(]\s*([\d.]+\s*%?)\s*,\s*([\d.]+\s*%?)\s*,\s*([\d.]+\s*%?)\s*(?:,\s*([\d.]+)\s*)?[)]$/m);if(o)return(a=t(r)).alpha=1,Object.assign(a,n(a)),new i(a);if(s&&s.length>0){var e;s.shift();var h=s[0],l=s[5]?parseFloat(s[5],10):1;return"rgb"===h?e=i.fromRGB:"hsl"===h&&(e=i.fromHSL),e(s[2],s[3],s[4],l)}},i.checkContrast=function(r,a){var t,n=h(r.toObject(),a.toObject());return n.max>=0&&n.min<3?t="fail":n.max>=3&&n.min<4.5?t="aa-large":n.max>=4.5&&n.min<7?t="aa":n.max>=7&&n.min<22&&(t="aaa"),{ratio:n.ratio,status:t}},i.__test__={hexToRgb:t,rgbToHsl:n,hslToRgb:o,layerColors:s,getLuminance:e,getContrast:h},r.namespace("Color",i,r)});
define("UWA/Fx",["UWA/Core","UWA/String","UWA/Class","UWA/Class/Options","UWA/Class/Events","UWA/Class/Timed","UWA/Element","UWA/Color"],function(t,n,i,r,e,u,a,o){"use strict";function s(t){return-1!==["borderColor","backgroundColor","color"].indexOf(n.camelCase(t))}function c(t){var n=Number(t);return isNaN(n)&&(n=parseInt(t,10)),isNaN(n)?0:n}var h=i.extend(r,u,e,{defaultOptions:{transition:"linear",duration:500,unit:"px",wait:!1},element:null,from:null,to:null,current:null,init:function(t,n){this.element=t,this.from={},this.to={},this.queue=[],this.setOptions(n)},tween:function(t,n,i){var r={};return r[t]=[n,i],this.start(r)},fade:function(t){t=void 0!==t?t:"toggle";var n=a.getOpacity.call(this.element),i={opacity:[]};switch(t){case"in":i.opacity=[n,1];break;case"out":i.opacity=[n,0];break;case"show":i.opacity=[1,1];break;case"hide":i.opacity=[0,0];break;case"toggle":i.opacity=n<1?[n,1]:[n,0];break;default:i.opacity=[n,t]}return this.start(i)},start:function(t){return this.options.wait&&this.hasAnimate("fx")?this.queue.push(t):(this.stop(),this.setSteps(t),this.dispatchEvent("onStart"),this.startTime=Date.now(),this.current={},this.animate()),this},pause:function(){return this.clearAnimate("fx"),this},stop:function(){return this.pause(),this.from={},this.to={},this},setSteps:function(t){var i,r={},e={};for(i in t)if(t.hasOwnProperty(i))if(i=n.camelCase(i),Array.isArray(t[i])?(r[i]=t[i][0],e[i]=t[i][1]):(r[i]=a.getStyle.call(this.element,i),e[i]=t[i]),s(i)){var u=o.parse(r[i]).toObject(),h=o.parse(e[i]).toObject();r[i]=[u.r,u.g,u.b,u.alpha],e[i]=[h.r,h.g,h.b,h.alpha]}else r[i]=c(r[i]),e[i]=c(e[i]);this.from=r,this.to=e},compute:function(i,r){var e,u=this.options,a=u.transition,o=u.duration,s=t.typeOf(a);if("string"===s){if(!t.is(h.Transitions[a],"function"))throw new Error("Invalid UWA.FX transition option value.");a=h.Transitions[a]}else if("array"===s)a=h.Transitions.cubicBezier.apply(null,a);else if("function"!==s)throw new Error("Invalid UWA.FX transition option value.");if(e=o>0&&i!==r?a(this.currentTime,i,r-i,o):r,isNaN(e))throw new Error(n.format('Invalid UWA.FX transition computation value with from "{0}" to "{1}".',i,r));return e},animate:function(){var t,n=Date.now(),i=this.options.duration,r=this.startTime;n<r+i?this.currentTime=n-r:(this.currentTime=i,t=!0),this.dispatchEvent("onAnimate",[this.element,this.from,this.to]),t?(this.stop(),this.dispatchEvent("onComplete"),this.queue.length>0&&this.start(this.queue.shift()),this.lastTime=null):this.setAnimate("fx",this.animate),this.fps=1e3/(n-(this.lastTime||n)),this.lastTime=n},onAnimate:function(t,n,i){var r,e,u={};for(r in n)n.hasOwnProperty(r)&&(e=s(r)?"rgba("+Math.round(this.compute(n[r][0],i[r][0]))+","+Math.round(this.compute(n[r][1],i[r][1]))+","+Math.round(this.compute(n[r][2],i[r][2]))+","+this.compute(n[r][3],i[r][3])+")":this.compute(n[r],i[r]),this.current[r]!==e&&(u[r]=e));this.current=u,a.setStyles.call(t,u)}});return h.Transitions={linear:function(t,n,i,r){return i*t/r+n},quadIn:function(t,n,i,r){return i*(t/=r)*t+n},quadOut:function(t,n,i,r){return-i*(t/=r)*(t-2)+n},quadInOut:function(t,n,i,r){return(t/=r/2)<1?i/2*t*t+n:-i/2*(--t*(t-2)-1)+n},cubicIn:function(t,n,i,r){return i*(t/=r)*t*t+n},cubicOut:function(t,n,i,r){return i*((t=t/r-1)*t*t+1)+n},cubicInOut:function(t,n,i,r){return(t/=r/2)<1?i/2*t*t*t+n:i/2*((t-=2)*t*t+2)+n},quartIn:function(t,n,i,r){return i*(t/=r)*t*t*t+n},quartOut:function(t,n,i,r){return-i*((t=t/r-1)*t*t*t-1)+n},quartInOut:function(t,n,i,r){return(t/=r/2)<1?i/2*t*t*t*t+n:-i/2*((t-=2)*t*t*t-2)+n},quintIn:function(t,n,i,r){return i*(t/=r)*t*t*t*t+n},quintOut:function(t,n,i,r){return i*((t=t/r-1)*t*t*t*t+1)+n},quintInOut:function(t,n,i,r){return(t/=r/2)<1?i/2*t*t*t*t*t+n:i/2*((t-=2)*t*t*t*t+2)+n},sineIn:function(t,n,i,r){return-i*Math.cos(t/r*(Math.PI/2))+i+n},sineOut:function(t,n,i,r){return i*Math.sin(t/r*(Math.PI/2))+n},sineInOut:function(t,n,i,r){return-i/2*(Math.cos(Math.PI*t/r)-1)+n},expoIn:function(t,n,i,r){return 0===t?n:i*Math.pow(2,10*(t/r-1))+n},expoOut:function(t,n,i,r){return t===r?n+i:i*(1-Math.pow(2,-10*t/r))+n},expoInOut:function(t,n,i,r){return 0===t?n:t===r?n+i:(t/=r/2)<1?i/2*Math.pow(2,10*(t-1))+n:i/2*(2-Math.pow(2,-10*--t))+n},circIn:function(t,n,i,r){return-i*(Math.sqrt(1-(t/=r)*t)-1)+n},circOut:function(t,n,i,r){return i*Math.sqrt(1-(t=t/r-1)*t)+n},circInOut:function(t,n,i,r){return(t/=r/2)<1?-i/2*(Math.sqrt(1-t*t)-1)+n:i/2*(Math.sqrt(1-(t-=2)*t)+1)+n},backIn:function(t,n,i,r,e){return i*(t/=r)*t*(((e=e||1.70158)+1)*t-e)+n},backOut:function(t,n,i,r,e){return i*((t=t/r-1)*t*(((e=e||1.70158)+1)*t+e)+1)+n},backInOut:function(t,n,i,r,e){return e=e||1.70158,(t/=r/2)<1?i/2*(t*t*((1+(e*=1.525))*t-e))+n:i/2*((t-=2)*t*((1+(e*=1.525))*t+e)+2)+n},elasticIn:function(t,n,i,r,e,u){var a;return 0===t?n:1==(t/=r)?n+i:(u=u||.3*r,(e=e||1)<Math.abs(i)?(e=i,a=u/4):a=u/(2*Math.PI)*Math.asin(i/e),-e*Math.pow(2,10*(t-=1))*Math.sin((t*r-a)*(2*Math.PI)/u)+n)},elasticOut:function(t,n,i,r,e,u){var a;return 0===t?n:1==(t/=r)?n+i:(u=u||.3*r,(e=e||1)<Math.abs(i)?(e=i,a=u/4):a=u/(2*Math.PI)*Math.asin(i/e),e*Math.pow(2,-10*t)*Math.sin((t*r-a)*(2*Math.PI)/u)+i+n)},elasticInOut:function(t,n,i,r,e,u){var a,o;return 0===t?o=n:2==(t/=r/2)?o=n+i:(u=u||r*(.3*1.5),(e=e||1)<Math.abs(i)?(e=i,a=u/4):a=u/(2*Math.PI)*Math.asin(i/e),o=t<1?e*Math.pow(2,10*(t-=1))*Math.sin((t*r-a)*(2*Math.PI)/u)*-.5+n:e*Math.pow(2,-10*(t-=1))*Math.sin((t*r-a)*(2*Math.PI)/u)*.5+i+n),o},bounceIn:function(t,n,i,r){return i-h.Transitions.bounceOut(r-t,0,i,r)+n},bounceOut:function(t,n,i,r){return(t/=r)<1/2.75?i*(7.5625*t*t)+n:t<2/2.75?i*(7.5625*(t-=1.5/2.75)*t+.75)+n:t<2.5/2.75?i*(7.5625*(t-=2.25/2.75)*t+.9375)+n:i*(7.5625*(t-=2.625/2.75)*t+.984375)+n},bounceInOut:function(t,n,i,r){var e=h.Transitions;return t<r/2?.5*e.bounceIn(2*t,0,i,r)+n:.5*e.bounceOut(2*t-r,0,i,r)+.5*i+n},quinticBezier:function(){return function(t,n,i,r,e,u){var a,o,s,c,h,f,l,p,b=u-t,m={a:b-(a=t)-(p=5*((e-t)/b+a)-20*((c=(r-t)/b)+(o=(n-t)/b))+30*(s=(i-t)/b))-(l=10*(c-a)+30*(o-s))-(f=10*(s-a)-4*(h=5*(o-a)))-h,b:p,c:l,d:f,e:h};return function(t,n,i,r){var e,u,a=t/r,o=a*a,s=o*t;return m.a||m.c?m.b||m.d?(e=o,u=o*a):u=s:(m.b||m.d)&&(e=s),n+i*(m.a*o+m.b*o+m.c*u+m.d*e+m.e*a)}}}(),cubicBezier:function(){function t(t,n){return((n.ax*t+n.bx)*t+n.cx)*t}function n(t,n){return(3*n.ax*t+2*n.bx)*t+n.cx}function i(i,r,e){return function(t,n){return((n.ay*t+n.by)*t+n.cy)*t}(function(i,r,e){var u,a,o,s,c,h,f;for(s=i,u=0;u<8;u++){if(c=t(s,r)-i,Math.abs(c)<e)return s;if(h=n(s,r),Math.abs(h)<e)break;s-=c/h}if(o=1,(s=i)<(a=0))f=a;else if(s>o)f=o;else{for(;a<o;){if(c=t(s,r),Math.abs(c-i)<e)return s;i>c?a=s:o=s,s=.5*(o-a)+a}f=s}return f}(i,r,e),r)}return function(t,n,r,e){var u,a,o,s,c,h,f={ax:1-(o=3*(u=t))-(s=3*(r-u)-o),bx:s,cx:o,ay:1-(c=3*(a=n))-(h=3*(e-a)-c),by:h,cy:c};return function(t,n,r,e){var u=t/e,a=function(t){return 1e3/60/t/4}(e),o=i(u,f,a);return n*(1-o)+(n+r)*o}}}()},t.namespace("Fx",h,t)});
define("UWA/Plugins/Abstract",["UWA/Core","UWA/Class","UWA/Class/Options"],function(n,t,e){"use strict";var i=t.extend(e,{init:function(n,t){this.widget=n,this.environment=n.environment,this.setOptions(t)},dispatchEvent:function(n,t,e){this.environment.dispatchEvent(n,t,e)},addEvent:function(n,t,e,i){this.environment.addEvent(n,t,e||this,i)},addEvents:function(n,t,e){var i;for(i in n)n.hasOwnProperty(i)&&this.addEvent(i,n[i],t,e)},removeEvent:function(n,t){this.environment.removeEvent(n,t)}});return n.namespace("Plugins/Abstract",i,n)});
define("UWA/Controls/Abstract",["vendors/webcomponents/MutationObserver","UWA/Core","UWA/Class","UWA/Class/Options","UWA/Class/Events","UWA/Utils"],function(t,e,n,o,r,i){"use strict";var s=[].forEach,a=new WeakMap,l=new WeakMap;function c(t,e){var n,o;for(n=0,o=t.length;n<o;n++){var r=t[n];if(1===r.nodeType){var i,s;e(r);var a=r.getElementsByTagName("*");for(i=0,s=a.length;i<s;i++)e(a[i])}}}function h(e){var n,o;try{o=(n=e&&(e.ownerDocument||e.document||e))&&n.documentElement}catch(t){}if(o&&!l.has(o)){var r=new t(function(t){function e(t,e,n){var o=a.get(t);o?o.dispatchEvent(e?"onInjected":"onRemoved",n):"IFRAME"===t.tagName&&h(t.contentWindow)}s.call(t,function(t){var n={nextSibling:t.nextSibling||null,previousSibling:t.previousSibling||null,parentNode:t.target};c(t.addedNodes,function(t){e(t,!0,n)}),c(t.removedNodes,function(t){e(t,!1,n)})})});l.set(o,r),r.observe(o,{childList:!0,subtree:!0})}}h(e.getGlobal());var u=n.extend(o,r,{elements:null,init:function(t){this.elements={},this.setOptions(t)},inject:function(t,e){var n=this.getContent();if(n){var o=a.get(n);if(o&&o!==this)throw new Error("This control container element is already owned by another control!");a.set(n,this),h(t),this.dispatchEvent("onPreInject",[t]),n.inject(t,e),this.dispatchEvent("onPostInject",[t]),this.dispatchEvent("onResize",[t])}return this},remove:function(){var t=this.getContent();return t&&t.remove(),this},getContent:function(){if(!this.elements.container&&!this.container)throw new Error("You don't have an elements.container or container.");return this.elements.container||this.container},getClassNames:function(){var t=this.constructor,e=i.toArray(arguments),n=this.options.className||"",o=i.splat(n).join(" ");for(e.length||(e=[""]),e.indexOf("")>=0&&!1!==this.options._root&&e.push("-root");t;)t.prototype.name&&(o+=" "+t.prototype.name+e.join(" "+t.prototype.name)),t=t.parent;return o},hide:function(){return this.getContent().hide(),this.dispatchEvent("onHide")},show:function(){return this.getContent().show(),this.dispatchEvent("onShow")},destroy:function(){var t,e=this.elements||{};for(t in this.container&&(e.container=this.container),this.elements.container&&a.delete(this.elements.container),e)e.hasOwnProperty(t)&&(e[t].destroy(),delete e[t]);this.removeEvents(),this.clearAllTimed&&this.clearAllTimed()}}),d=new WeakMap;return u._getClosestControlFromElement=function(t){for(;t;){var e=d.get(t);if(e)return e;t=t.parentNode}return null},u._getClosestControlsFromElement=function(t){for(var e=[];t;){var n=d.get(t);n&&e.indexOf(n)<0&&e.push(n),t=t.parentNode}return e},u._linkElementToControl=function(t,e){var n=d.get(e);if(n){if(n!==t)throw new Error("This element is already linked to another control")}else d.set(e,t)},e.namespace("Controls/Abstract",u,e)});
define("UWA/Controls/Pager",["UWA/Core","UWA/Event","UWA/Controls/Abstract"],function(t,e,n){"use strict";var i=n.extend({offset:0,limit:0,max:0,length:0,loadingData:!1,defaultOptions:{className:"uwa-pager nv-pager",type:0,showPageLinks:!1,showMoreLink:!1,pageLinks:5,length:0,offset:0,limit:10,max:0,loadNext:null,prevLabel:"prev",nextLabel:"next",moreLabel:"more"},init:function(t){this._parent(t),t=this.options,this.offset=parseInt(t.offset,10),this.limit=parseInt(t.limit,10),this.max=parseInt(t.max,10),this.length=parseInt(t.length,10),this.buildSkeleton()},setOptions:function(t){return this._parent(t),(t=this.options).dataLength?t.length=t.dataLength:t.dataArray&&(t.length=t.dataArray.length),t.onChange&&this.addEvent("onOffsetChange",t.onChange),t.onMoreClick&&this.addEvent("onMoreClick",t.onMoreClick),(t.showPageLinks||t.pageLinks&&!t.type)&&(this.type=1),this},setLength:function(t){this.length=parseInt(t,10),this.setOffset(this.offset)},setOffset:function(t){var e=this.offset;return t=t<0?0:t,this.offset=Math.min(parseInt(t,10),this.max||this.length),e!==this.offset&&this.dispatchEvent("onOffsetChange",[this.offset]),this},setLimit:function(t){return this.limit=parseInt(t,10),this},getPageOffset:function(t){return Math.ceil((parseInt(t,10)||this.offset)/this.limit)},getPages:function(){return Math.ceil((this.max||this.length||1)/this.limit)},isLastPage:function(){var t=!this.max||this.length>=this.max,e=this.offset+this.limit>=this.length;return t&&e},buildSkeleton:function(){this.elements.container=t.createElement("div",{class:this.options.className}),this.dispatchEvent("onRefresh")},buildPageInfos:function(){var e=this.elements;e.pageInfos=t.createElement("span",{class:"pageInfos",html:t.createElement("span",{text:this.getPageOffset()+1+" / "+this.getPages()})}).inject(e.subContainer)},buildPageLinks:function(){var e,n,i=this.elements,s=this.options,a=this.injectPageLink.bind(this),o=this.injectPageSeparator.bind(this),h=s.pageLinks,l=this.getPages(),r=this.getPageOffset(),c=0,f=Math.round(h/2),g=r>=f&&l>=h?r-f+1:0;if(i.pageContainer=t.createElement("span",{class:"pageLinks"}),g<l)for(e=g;e<l&&c<h;e++)g>=1&&0===c&&(a(c),e>1&&o()),n=a(e),e===r&&n.addClassName("selected"),e<l-1&&c===h-1&&(e<l-2&&o(),a(l-1)),c++;i.pageContainer.inject(i.subContainer)},injectPageLink:function(e){var n=parseInt(e+1,10);return t.createElement("a",{class:"pageLink",href:"#page_"+n,text:n,events:{click:this.dispatchAsEventListener("onPageClick",e)}}).inject(this.elements.pageContainer)},injectPageSeparator:function(){return t.createElement("span",{class:"comas",text:" ... "}).inject(this.elements.pageContainer)},onRefresh:function(){var e=this.elements,n=this.options,i=this.isLastPage();e.container.empty(),e.subContainer=t.createElement("div"),e.prev=t.createElement("a",{class:"prev"+(0===this.offset?" disabled":""),href:"#prev",html:t.createElement("span",{text:t.i18n(n.prevLabel)}),events:{click:this.dispatchAsEventListener("onPrevClick")}}).inject(e.subContainer),i&&(n.showMoreLink||n.moreLink)?e.next=t.createElement("a",{class:"more",href:n.moreLink||"#more",html:t.createElement("span",{text:t.i18n(n.moreLabel)}),events:{click:this.dispatchAsEventListener("onMoreClick")}}).inject(e.subContainer):e.next=t.createElement("a",{class:"next"+(i?" disabled":""),href:"#next",html:t.createElement("span",{text:t.i18n(n.nextLabel)}),events:{click:this.dispatchAsEventListener("onNextClick")}}).inject(e.subContainer),1===n.type?this.buildPageLinks():2===n.type&&this.buildPageInfos(),e.subContainer.inject(e.container)},onOffsetChange:function(t){this.offset=t,this.dispatchEvent("onRefresh"),this.dispatchEvent("onChange",[t])},onPageClick:function(e,n){t.Event.preventDefault(e),this.loadingData||this.setOffset(this.limit*n)},onPrevClick:function(t){e.preventDefault(t);var n=e.findElement(t,"a");this.loadingData||n.hasClassName("disabled")||this.setOffset(this.offset-this.limit)},onNextClick:function(t){e.preventDefault(t);var n=this,i=n.options.loadNext,s=e.findElement(t,"a"),a=n.offset+n.limit,o=a+n.limit<=n.length;function h(){n.setOffset(a)}n.loadingData||n.isLastPage()||s.hasClassName("disabled")||(!i&&n.onNeedMoreData&&(i=function(t,e){n.onNeedMoreData(t),setTimeout(e.bind(null,null),6e4)}),!o&&i?(n.dispatchEvent("onLoadingStart"),i(n.length,function(t){t&&(n.length=t),h(),n.dispatchEvent("onLoadingEnd")})):h())},onMoreClick:function(){},onLoadingStart:function(){this.loadingData=!0,this.elements.subContainer.addClassName("loading")},onLoadingEnd:function(){this.loadingData=!1,this.elements.subContainer.removeClassName("loading")}});return t.namespace("Controls/Pager",i,t)});
define("UWA/Controls/Img",["UWA/Core","UWA/Controls/Abstract"],function(e,t){"use strict";var i=t.extend({defaultOptions:{className:"uwa-img",url:null,height:null,width:null},init:function(e){this._parent(e),this.buildSkeleton()},buildSkeleton:function(){var t=this.options,i=this.elements;i.container=e.createElement("div",{class:t.className,styles:{width:t.width+"px",height:t.height+"px"}}),(i.image=e.createElement("img",{src:t.url,width:"100%",height:"100%",events:{error:this.dispatchAsEventListener("onError"),load:this.dispatchAsEventListener("onLoad"),resize:this.dispatchAsEventListener("onResize")}})).inject(i.container)}});return e.namespace("Controls/Img",i,e)});
define("UWA/Utils/Scroll",["vendors/webcomponents/WeakMap","UWA/Core","UWA/Element","UWA/Fx","UWA/Event"],function(e,t,o,l,n){"use strict";function r(e){return"body"===o.getTagName.call(e)}function i(e,t){var l=o.getStyle.call(e,t?"overflow-"+t:"overflow");return r(e)||"scroll"===l||"auto"===l}function a(e,t){for(;e&&1===e.nodeType&&!i(e,t);)e=e.parentNode;return e}function c(e,t){return a(e&&e.parentNode,t)}function s(e){r(e)&&(e=o.getWindow.call(e));var l=o.getScrolls.call(e);return t.owns(l,"x")&&(l.left=l.x,l.top=l.y),l}function f(e,l){r(e)&&(e=o.getWindow.call(e));var n=s(e);t.is(l.left)||(l.left=n.left),t.is(l.top)||(l.top=n.top),t.is(e,"window")?e.scrollTo(l.left,l.top):(e.scrollTop=l.top,e.scrollLeft=l.left)}var p=l.extend({setSteps:function(e){var t,o={},l={},n=s(this.element);for(t in e)Array.isArray(e[t])?(o[t]=e[t][0],l[t]=e[t][1]):(o[t]=n[t],l[t]=e[t]);this.from=o,this.to=l},onAnimate:function(e,t,o){var l,n={};for(l in t)n[l]=this.compute(t[l],o[l]);f(e,n)}}),u=new e;function m(e,o,l){l=t.extend({onComplete:null},l);var n=u.get(e);n&&(n.stop(),n.dispatchEvent("onComplete")),n=new p(e,{transition:"sineOut",duration:n?100:200,events:{onComplete:function(){u.delete(e),l.onComplete&&l.onComplete()}}}),u.set(e,n),n.start(o)}return t.namespace("Utils/Scroll",{scrollToElement:function(e,l){var n=(l=t.extend({top:!1,bottom:!1,margin:0,scrollable:null,smooth:!1,onComplete:null},l)).scrollable||c(e);if(n){var i=r(n),a=i?o.getSize.call(o.getWindow.call(e)):{width:n.clientWidth,height:n.clientHeight},p=o.getSize.call(e),u=o.getOffsets.call(e),g={top:u.y,left:u.x,bottom:0,right:0},h=s(n);[0,1].forEach(function(e){var t=e?"top":"left",r=e?"bottom":"right",c=e?"height":"width";g[t]-=i?h[t]:o.getOffsets.call(n)[e?"y":"x"],g[t]-=l.margin,g[r]=a[c]-g[t]-p[c]-2*l.margin;var s=g[t]<0||g[r]<0&&g[r]<-g[t],f=g[r]<0;l[r]||!s&&!l[t]?(l[r]||f)&&(h[t]-=g[r]):h[t]+=g[t]}),l.smooth?m(n,h,{onComplete:l.onComplete}):(f(n,h),l.onComplete&&l.onComplete())}},smoothScroll:m,preventParentScroll:function(e,t){var l=function(e,t){var o=a(n.getElement(t)),l=!1;if(this.isInjected(o))l=!0;else{var r=o.scrollHeight,i=o.clientHeight,c=o.scrollTop,s=n.wheelDelta(t);(i!==r||e&&!1===e.onlyScrollable)&&(s<0&&!(c+i<r)||s>0&&!(c>0))&&(l=!0)}l&&n.stop(t)}.bind(e,t);return o.addEvent.call(e,"mousewheel",l),function(){o.removeEvent.call(e,"mousewheel",l)}},getClosestScrollable:a,getParentScrollable:c},t)});
define("UWA/Controls/DropDown",["UWA/Core","UWA/Event","UWA/Element","UWA/Controls/Abstract","UWA/Utils/Client","UWA/Utils/Scroll"],function(t,e,n,i,o,s){"use strict";var l,r=o.Features.eventCapture;return(l=i.extend({name:"uwa-dropdown",defaultOptions:{position:{},positionOptions:{boundary:"auto"},global:!1},init:function(t){this._parent(t),this.clickOutsideEvent=function(t){var n=t&&e.getElement(t),o=this.elements.container,s=n.isInjected(o),l=i._getClosestControlsFromElement(n).some(function(t){return t.getContent().isInjected(o)});s||l||this.dispatchEvent("onClickOutside",[t])}.bind(this)},destroy:function(){this.hide(),this._parent()},getContent:function(){var n=this.elements;return n.container||(n.container=t.createElement("div",{class:this.getClassNames()+(this.options.global?" global":""),events:{click:this.dispatchEvent.bind(this,"onClick"),mouseleave:this.dispatchEvent.bind(this,"onMouseLeave")}}),this.options.global?(n.bacon=t.createElement("div",{class:this.getClassNames("-bacon")}).hide(),this._scrollPrevention=function(t){var n=e.getElement(t),i=this.getInnerElement();i===n||n.isInjected(i)||e.preventDefault(t)}.bind(this),s.preventParentScroll(n.container,{onlyScrollable:!1})):n.container.hide(),i._linkElementToControl(this,n.container),r||(n.capture=t.createElement("div",{styles:{width:"100%",height:"100%",position:"absolute",zIndex:1e3,top:0,left:0},events:{click:this.clickOutsideEvent}}))),n.bacon||n.container},onClick:function(t){e.stopPropagation(t),this.hide()},onPostInject:function(){this.updatePosition()},onShow:function(){this.options.global&&(this.elements.container.inject(document.body),n.addEvent.call(document.body,"mousewheel",this._scrollPrevention,null,!0)),this.updatePosition(),this.hasEvent("onClickOutside")&&(r?n.addEvent.call(document,"click",this.clickOutsideEvent,null,0,!0):this.elements.capture.inject(document.body))},onHide:function(){this.options.global&&(this.elements.container.remove(),n.removeEvent.call(document.body,"mousewheel",this._scrollPrevention,!0)),r?n.removeEvent.call(document,"click",this.clickOutsideEvent,!0):this.elements.capture.remove()},onRemoved:function(){var t=this.elements,e=t.bacon||t.container;e&&e.hide(),this.options.global&&t.container&&t.container.remove(),this._scrollPrevention&&n.removeEvent.call(document.body,"mousewheel",this._scrollPrevention,!0)},isOpen:function(){return!!this.elements.container&&"none"!==this.getContent().getStyle("display")},toggle:function(e){return t.is(e)||(e=!this.isOpen()),this[e?"show":"hide"](),this},setPosition:function(e,n){return t.extend(this.options,{position:e,positionOptions:n||{}},!0),this.updatePosition()},updatePosition:function(){function e(e){return t.is(e,"function")?e():e}return function(){return this.isOpen()&&(this.dispatchEvent("onPreUpdatePosition"),this.elements.container.setPosition(e(this.options.position),e(this.options.positionOptions))),this}}(),getInnerElement:function(){return this.getContent(),this.elements.container}})).Pointy=l.extend({name:"uwa-pointydropdown",defaultOptions:{autoPosition:["below-center","right-center","left-center","above-center"],margin:12},updatePosition:function(){this.dispatchEvent("onPreUpdatePosition");var e,n,i,o,s=this.options,l=s.margin;return e=s.target?s.target.getDimensions():{width:0,height:0},n=this.elements.container.getDimensions(),i=s.autoPosition.map(function(t){var i=(t=t.split("-"))[0],o=t[1]||"center",r={x:0,y:0};return r.place=i,r.align=o,"below"===i?r.y=e.height+l:"above"===i?r.y=-n.outerHeight-l:"center"===o?r.y=e.height/2-n.outerHeight/2:"end"===o&&(r.y=Math.max(e.height,30)-n.outerHeight),"left"===i?r.x=-n.outerWidth-l:"right"===i?r.x=e.width+l:"center"===o?r.x=e.width/2-n.outerWidth/2:"end"===o&&(r.x=Math.max(e.width,30)-n.outerWidth),s.target||(r.x+=s.position.x||0,r.y+=s.position.y||0,"center"!==o&&("right"!==i&&"left"!==i||(r.y-=15),"above"!==i&&"below"!==i||(r.x-=15))),r}),this.isOpen()&&((o=this.elements.container).setPosition(i,t.merge({relative:s.target},this.options.positionOptions)),i=i[0],this._containerClassName&&o.removeClassName(this._containerClassName),this._containerClassName=i.place+" "+i.align,o.addClassName(this._containerClassName),this.updatePointPosition(i.place)),this},updatePointPosition:function(t){var e=this.options.target,n=this.elements.container,i=n.getSize(),o=n.getOffsets(),s=e?e.getSize():{height:0,width:0},l=e?e.getOffsets():this.options.position,r={bottom:null,left:null,right:null,top:null};l.x-=o.x,l.y-=o.y,"below"===t||"above"===t?(r.left=l.x+s.width/2,(r.left<10||r.left>i.width-10)&&(r.left=i.width/2),"below"===t?r.top=0:r.bottom=0):(r.top=l.y+s.height/2,(r.top<10||r.top>i.height-10)&&(r.top=i.height/2),"right"===t?r.left=0:r.right=0),this.elements.point.setStyles(r).setText({above:"j",below:"k",left:"m",right:"l"}[t]||" ").toggleClassName("side","left"===t||"right"===t)},getInnerElement:function(){return this.getContent(),this.elements.inner},getContent:function(){var e=this.elements,n=this._parent();return e.inner||e.container.setContent(e.inner=t.createElement("div",{class:this.getClassNames("-inner")}),e.point=t.createElement("div",{class:this.getClassNames("-point")})),n}}),t.namespace("Controls/DropDown",l,t)});
define("UWA/Controls/Drag",["UWA/Internal/Deprecate","UWA/Core","UWA/Class","UWA/Class/Options","UWA/Utils","UWA/Utils/Client","UWA/Element","UWA/Event"],function(t,e,i,s,o,n,h,a){"use strict";var r,l=n.Features.eventCapture,c=function(){};function d(t){return t.type.startsWith("touch")}function p(t,e){var i,s=t.offsetParent;s&&1===s.nodeType?((i=h.getOffsets.call(s)).y+=parseInt(h.getStyle.call(s,"border-top-width"),10)||0,i.x+=parseInt(h.getStyle.call(s,"border-left-width"),10)||0):i={x:0,y:0},t.setStyles({top:e.y-i.y+"px",left:e.x-i.x+"px"})}function u(t){for(var e,i=h.getComputedSize;t&&"inline"===h.getStyle.call(t,"display");)t=t.getParent();return t?((e=h.getOffsets.call(t)).maxX=e.x+t.offsetWidth-i.call(t,"border-right-width","padding-right"),e.maxY=e.y+t.offsetHeight-i.call(t,"border-bottom-width","padding-bottom"),e.x+=i.call(t,"border-left-width","padding-left"),e.y+=i.call(t,"border-top-width","padding-top")):e={x:0,y:0,maxX:0,maxY:0},e}return(r=i.extend(s,{defaultOptions:{mouseSnap:10,mouseDelay:0,touchSnap:20,touchDelay:300,delegate:"*",document:document},init:function(e){this.setOptions(e),void 0!==this.options.snap&&(t.warn("Controls/Drag snap option","Use the mouseSnap and touchSnap options instead."),this.options.mouseSnap=this.options.touchSnap=this.options.snap),void 0!==this.options.delay&&(t.warn("Controls/Drag delay option","Use the mouseDelay and touchDelay options instead."),this.options.mouseDelay=this.options.touchDelay=this.options.delay);var i=this.onMove.bind(this),s=this.onStop.bind(this),o=this.onStart.bind(this);this.documentEvents={touchmove:i,mousemove:i,touchend:s,mouseup:s,touchcancel:s},this.elementEvents={touchstart:o,mousedown:o},this.attach()},setOptions:function(t){return this._parent(t),t=this.options,this.root=e.extendElement(t.root||document.body),this.element=e.extendElement(t.element||this.root),this.document=t.document,l||(this.clickDiscarder||(this.clickDiscarder=e.createElement("div",{styles:{position:"absolute",height:"1px",width:"1px"}})),this.clickDiscarder.inject(this.root)),this},destroy:function(){this.detach(),l||this.clickDiscarder.destroy()},attach:function(){return h.addEvents.call(this.element,this.elementEvents),this},detach:function(){return this.reset(),h.removeEvents.call(this.element,this.elementEvents),this},start:c,move:l?c:function(t){p(this.clickDiscarder,t)},snap:function(t){l||(p(this.clickDiscarder,t),this.clickDiscarder.show());var i=e.Controls&&e.Controls.Scroller;(i=i&&i.activeScroller)&&i.onScrollStop(this.currentEvent)},stop:c,cancel:c,reset:function(){clearTimeout(this.startTimeout),l?this.snapped&&(this.document.addEventListener("click",a.stopPropagation,!0),setTimeout(function(){this.document.removeEventListener("click",a.stopPropagation,!0)}.bind(this),300)):this.clickDiscarder.hide(),this.snapped=!1,this.startOrigin=this.currentDelta=this.currentEvent=this.target=null,h.removeEvents.call(this.document,this.documentEvents)},onStart:function(t){var e=a.getElement(t);if((t.which||t.button||0)<2&&!this.target&&h.match.call(e,this.options.delegate,this.root)&&(this.currentEvent=t,this.target=e,this.startOrigin=a.getPosition(t),this.start(this.startOrigin),this.target)){h.addEvents.call(this.document,this.documentEvents);var i=d(t)?this.options.touchDelay:this.options.mouseDelay;i&&(this.startTimeout=setTimeout(this.onMove.bind(this,!1),i)),d(t)||a.preventDefault(t)}},onMove:function(t){var e,i;t?(this.currentEvent=t,this.snapped&&a.preventDefault(t)):(t=this.currentEvent,i=!0);var s=a.getPosition(t);if(this.currentDelta=e={x:s.x-this.startOrigin.x,y:s.y-this.startOrigin.y,distance:0},e.distance=Math.sqrt(e.x*e.x+e.y*e.y),!this.snapped){var o=d(t)?this.options.touchSnap:this.options.mouseSnap,n=d(t)?this.options.touchDelay:this.options.mouseDelay;(n?i&&e.distance<=o:!o||e.distance>o)?(this.snapped=!0,this.snap(s,e)):n&&(this.cancel(),this.reset())}this.snapped&&this.move(s,e)},onStop:function(t){this.currentEvent=t,this.snapped?(this.stop(),a.stop(t)):this.cancel(),this.reset()}})).Move=r.extend({init:function(t){this._parent(t),this.refreshCache=this.refreshCache.bind(this)},setOptions:function(t){return t&&!t.root&&(t.root=t.container),this._parent(t)},start:function(t){this._parent(t),this.context=Object.create(this),!1!==this.call("start")&&!0!==this.call("fixed",this.target)||this.reset()},snap:function(t,i){this._parent(t,i);var s,o=this.options;this.handles=this.call("handles")||this.target,o.centerHandles&&p(this.handles,{x:t.x-this.handles.offsetWidth/2-i.x,y:t.y-this.handles.offsetHeight/2-i.y}),this.startPosition=h.getOffsets.call(this.handles),this.options.overlay&&(s=this.document.body||this.document,this.overlay=e.createElement("div",{styles:{position:"absolute",top:0,left:0,width:s.offsetWidth+"px",height:s.offsetHeight+"px"}}).inject(s)),this.refreshCache()},refreshCache:function(){var t=this.options;if(this.zones=t.zones?this.getList(t.zones):[this.root],this.positions=this.zones.map(function(t){var e=u(t);return e.element=t,e}),t.container&&this.handles){var e=u(t.container),i=h.getDimensions.call(this.handles);this.limit={x:[e.x,e.maxX-i.outerWidth],y:[e.y,e.maxY-i.outerHeight]}}else this.limit={x:[-1/0,1/0],y:[-1/0,1/0]}},reset:function(){this._parent(),this.zone=null,this.startPosition=null,this.overlay&&(this.overlay.destroy(),this.overlay=null)},stop:function(){this._parent(),this.zone&&!1!==this.call("drop")||(this.setPosition(this.startOrigin,{x:0,y:0}),this.call("cancel")),this.call("stop")},move:function(t,e){var i,s,o,n;for(this._parent(t,e),this.setPosition(t,e),i=0,s=this.positions.length;i<s;i+=1)(n=this.positions[i]).x<=t.x&&t.x<=n.maxX&&n.y<=t.y&&t.y<=n.maxY&&(o=n.element);this.zone!==o&&(this.zone&&(this.call("leave"),this.placeholder&&(this.placeholder.remove(),this.placeholder=null,this.refreshCache())),this.zone=o,o&&(this.placeholder=this.call("enter"),this.refreshPlaceholderCache())),this.zone&&this.placeholder&&this.placePlaceholder(),this.call("move")},setPosition:function(t,e){var i,s,o,n,h=this.limited={},a={};for(s=0;s<2;s+=1)o=s?"x":"y",i=this.limit[o],a[o]=this.startPosition[o]+e[o],n=0,i[1]<a[o]?(n=i[1]-a[o],h[s?"right":"bottom"]=n):i[0]>a[o]&&(n=i[0]-a[o],h[s?"left":"top"]=n),n&&(t[o]+=n,a[o]+=n,e[o]+=n);p(this.handles,a)},getList:function(t){var i=e.typeOf(t);return"array"===i?t:"function"===i?t.apply(this,Array.prototype.slice.call(arguments,1)):this.root.getElements(t)},call:function(t,e){var i=this.options[t];if(i)return o.attempt(i,0,null,this.context,e)},refreshPlaceholderCache:function(){var t,e,i,s=(this.zone||this.root).childNodes,o=[];for(e=0,i=s.length;e<i;e+=1)1===(t=s[e]).nodeType&&t!==this.handles&&t!==this.placeholder&&(t.offsetHeight||t.offsetWidth)&&this.clickDiscarder!==t&&!0!==this.call("fixed",t)&&(o[o.length]={element:t,position:h.getOffsets.call(t)});this.placeholderCache=o},placePlaceholder:function(){for(var t,e,i,s,o,n,a,r,l,c,d,p,u,f="offsetWidth",m=this.context.handles,v=this.context.placeholder,y=this.context.limited,g=this.zone||this.root,x=this.target,D=this.placeholderCache;x&&x.parentNode!==g;)x=x.parentNode;for(t=h.getOffsets.call(m),l={x:y.left?-1/0:y.right?1/0:t.x+m[f]/2,y:y.top?-1/0:y.bottom?1/0:t.y+m.offsetHeight/2},e=0,i=D.length;e<i;e+=1)t=(s=D[e]).position,(p=void 0===u||u>t.x)?d=void 0===u:c=!0,u=t.x+s.element[f],(p||t.x<=l.x)&&(d||t.y<=l.y)&&(o=e);n=0,void 0!==o&&(t=(s=D[o]).position,n=(c?t.x+s.element[f]/2>l.x:t.y+s.element.offsetHeight/2>l.y)?o:o+1),a=D[n]&&D[n].element,r=D[n-1]&&D[n-1].element,x===m||!x||this.options.allowBesidePlaceholder||r!==x&&a!==x?(a?a!==v&&a.previousSibling!==v:r?r!==v&&r.nextSibling!==v:g.lastChild!==v)&&(a||r?v.inject(a||r,a?"before":"after"):v.inject(g),this.refreshPlaceholderCache(),this.refreshCache()):h.isInjected.call(v)&&(v.remove(),this.refreshPlaceholderCache(),this.refreshCache())}}),e.namespace("Controls/Drag",r,e)});
define("UWA/Controls/ThemedScroller",["UWA/Core","UWA/Utils","UWA/Utils/Client","UWA/Controls/Abstract","UWA/Controls/Drag","UWA/Class/Timed"],function(t,e,s,i,o,n){"use strict";var l=!1;function r(){if(!1!==l)return l;var e=t.createElement("div",{class:"uwa-themed-scroller-content no-native-scrollbars",styles:{width:"100px",height:"100px",position:"absolute",visibility:"hidden",top:"0",left:"0",overflow:"scroll"}});return document.body.appendChild(e),l=e.offsetWidth-e.clientWidth,document.body.removeChild(e),l}function a(t){t.event&&(t=t.event);var e,s=t.changedTouches||t.touches||[t],i={x:0,y:0},o=s.length;for(e=0;e<o;e++)i.x+=s[e].clientX/o,i.y+=s[e].clientY/o;return i}var c={delta:0,coef:1,active:!1,visible:!1,scrollSize:0,scrollPosition:0,offsetSize:0},h=o.extend({defaultOptions:{touchSnap:0,touchDelay:0},init:function(t,e){this._parent(e),this.scroller=t,this.direction=this.element.className.contains("scrollbar-y")?"y":"x"},_getInfos:function(){return this.scroller._infos[this.direction]},_getPosition:function(){var t=this.element.getBoundingClientRect()["y"===this.direction?"top":"left"];return a(this.currentEvent)[this.direction]-t},start:function(t){this._parent(t),this._getInfos().active=!0,this.scroller.update(),this.position=this._getPosition()},move:function(t,e){this._parent(t,e);var s=this._getInfos();s.delta=(this._getPosition()-this.position)*s.coef,s.active=!0,this.scroller.updateVisible()},stop:function(){this._parent(),this.scroller.updateActive(this.currentEvent)}}),d=i.extend(n,{name:"uwa-themed-scroller",options:{element:null,scrollbars:"auto",scrollbarsMargin:4,scrollbarsMinSize:50,shadows:!1},init:function(e){t.is(e)&&t.is(e.element)&&t.extendElement(e.element),this._parent(e),this._elementEvents={mousemove:this.updateActive.bind(this),mouseout:this.updateActive.bind(this)},"auto"===this.options.scrollbars&&(this.options.scrollbars=0===r()?"native":"virtual"),this._buildElements(),this._initElements(),this.initInfos()},initInfos:function(){this._infos={x:Object.create(c),y:Object.create(c)},this.setPeriodical("update",this.update,1e3),this.update()},destroy:function(){if(this.options.element){var t=this.elements.container;t.removeEvents(this._elementEvents).removeClassName(this.getClassNames()).setContent(this.elements.content.childNodes);var e=t.destroy;t.destroy=function(){},this._parent(),t.destroy=e}else this._parent()},onInjected:function(){this.initInfos()},_buildElements:function(){var e=this.options.element||t.createElement("div");this.elements.container=e,this.elements.content=t.createElement("div",{html:e.childNodes}).inject(e)},_initElements:function(){var t=this.elements.container,e=this.elements.content;t.addClassName(this.getClassNames()).addEvents(this._elementEvents);var s="native"===this.options.scrollbars,i=s?"native-scrollbars ":"no-native-scrollbars ";e.addClassName(i+this.getClassNames("-content")).addEvent("scroll",this.updateVisible.bind(this)),s||e.setStyles({right:-r(),bottom:-r()})},getInnerElement:function(){return this.elements.content},getScrollbar:function(e,s){var i=this.elements[e+"Scrollbar"];return!i&&s&&(i=this.elements[e+"Scrollbar"]=t.createElement("div",{class:this.getClassNames("-scrollbar","-scrollbar-"+e)}).inject(this.elements.container),new h(this,{element:i,root:this.elements.container}),i.clientHeight),i},getShadow:function(e,s){var i=this.elements[e+"Shadow"];return!i&&s&&(i=this.elements[e+"Shadow"]=t.createElement("div",{class:this.getClassNames("-shadow","-shadow-"+e)}).inject(this.elements.container)),i},showShadow:function(t,e){var s=this.getShadow(t,e);e?(e>100&&(e=100),s.setStyle("opacity",e/100).addClassName("active")):s&&s.removeClassName("active")},updateActive:function(t){if("virtual"===this.options.scrollbars){if("mouseout"===t.type||"touchend"===t.type)this._infos.x.active=this._infos.y.active=!1;else{var e=this.elements.container.getBoundingClientRect(),s=a(t);["x","y"].forEach(function(t,o){var n=e[o?"right":"bottom"];this._infos[t].active=i(n-12,s[o?"x":"y"],n)&&i(e[o?"top":"left"],s[t],e[o?"bottom":"right"])},this)}this.updateVisible()}function i(t,e,s){return t<e&&e<s}},updateVisible:function(){this._infos.x.visible=this._infos.y.visible=!0,this.setDelayed("scrollbars-visible",function(){this._infos.x.visible=this._infos.y.visible=!1,this.update()},1e3),this.update()},_read:function(t){var e=this._infos[t?"y":"x"],s=this.elements.content,i=r();e.scrollSize=s[t?"scrollHeight":"scrollWidth"],e.scrollPosition=s[t?"scrollTop":"scrollLeft"]+e.delta,e.offsetSize=s[t?"offsetHeight":"offsetWidth"]-i,e.scrollPosition<0?e.scrollPosition=0:e.scrollPosition>e.scrollSize-e.offsetSize&&(e.scrollPosition=e.scrollSize-e.offsetSize)},_write:function(t){var e=t?"y":"x",s=this._infos[e],i=this.options;if(s.delta&&(this.elements.content[t?"scrollTop":"scrollLeft"]=s.scrollPosition,s.delta=0),"virtual"===this.options.scrollbars){var o=s.scrollSize>s.offsetSize+1,n=this.getScrollbar(e,o);if(o&&s.scrollSize){var l=s.offsetSize-2*i.scrollbarsMargin,r=l*(s.offsetSize/s.scrollSize);r<i.scrollbarsMinSize&&(r=i.scrollbarsMinSize),s.coef=(s.scrollSize-s.offsetSize)/(l-r),n.style[t?"top":"left"]=i.scrollbarsMargin+s.scrollPosition/s.coef+"px",n.style[t?"height":"width"]=r+"px",n.toggleClassName("active",s.active).toggleClassName("visible",s.visible)}else n&&n.removeClassName("active").removeClassName("visible")}i.shadows&&s.offsetSize&&(this.showShadow(e+"-start",s.scrollPosition),this.showShadow(e+"-end",s.scrollSize-s.scrollPosition-s.offsetSize))},update:function(){this.setAnimate("update",function(){this._read(!1),this._read(!0),t.equals(this._previousInfos,this._infos)||(this._write(!1),this._write(!0),this._previousInfos=t.clone(this._infos))})}});return t.namespace("Controls/ThemedScroller",d,t)});
define("UWA/Controls/Input",["UWA/Core","UWA/Event","UWA/Element","UWA/Utils","UWA/Utils/Client","UWA/Utils/Scroll","UWA/Controls/Abstract","UWA/Controls/DropDown","UWA/Controls/ThemedScroller","UWA/Class/Timed"],function(e,t,n,s,i,o,l,a,c,r){"use strict";var u=l.extend({options:{className:"",element:null,attributes:{},value:"",clickable:!0,mixed:!1},name:"uwa-input",_hiddenInput:!0,init:function(t){if(this.constructor===u)throw new Error("Use a subclass of Input");this._parent(t);var n=t&&t.element,s=n&&n.parentNode,i=n&&n.nextSibling;s&&s.removeChild(n),this.events=null,this.getContent(),e.owns(t,"value")&&this.setValue(t.value),s&&this.inject(i||s,i&&"before")},buildSkeleton:function(){var t=this.elements;this._hiddenInput?(t.input=this.options.element||this.buildInput(),t.content=e.createElement("div",{class:this.getClassNames("-content")}),t.input.addClassName(this.getClassNames("-input")+" hidden-input"),t.container=(this.options.container||e.createElement("div")).addContent(t.input,t.content)):t.content=t.container=t.input=this.options.element||this.options.container||this.buildInput(),t.input.set(this.options.attributes),t.container.addClassName(this.getClassNames()),this.options.clickable||this.elements.container.addClassName("not-clickable"),this.setDisabled(this.isDisabled())},_syncEvents:function(e){var t=this,n=this.elements;function s(e){return t.dispatchEvent.bind(t,e)}t.events||(t.events={container:{mouseenter:s("onMouseEnter"),mouseleave:s("onMouseLeave"),mousedown:function(e){this.addClassName("active"),t.dispatchEvent("onMouseDown",[e])},mouseup:function(){this.removeClassName("active")},click:s("onClick")},input:{change:s("onChange"),keydown:s("onKeyDown"),focus:t.focus.bind(t,!0,!1),blur:t.focus.bind(t,!1,!1)}}),t.isDisabled()?(n.container.removeEvents(t.events.container),n.input.removeEvents(t.events.input)):(t._hiddenInput&&e||n.container.addEvents(t.events.container),n.input.addEvents(t.events.input))},buildInput:function(){return e.createElement("input",{type:"text"})},syncInput:function(){this._hiddenInput&&this.elements.content&&this.elements.content.setText(this.getValue())},focus:function(e,t){return void 0===e&&(e=!0),n.toggleClassName.call(this.elements.container,"focus",e),!1!==t&&this.elements.input[e?"focus":"blur"](),this},isDisabled:function(){return Boolean(this.elements.input.disabled)},setDisabled:function(e){return void 0===e&&(e=!0),this.elements.input.disabled=e,this.elements.container.toggleClassName("disabled",e),this._syncEvents(),this},getValue:function(){var e=this.elements.input,t=e.getTagName();return"input"===t||"textarea"===t?e.value:e.getText()},setValue:function(e){var t=this.elements.input,n=t.getTagName();return"input"===n||"textarea"===n?t.value=e:t.setText(e),this.syncInput(),this},getContent:function(){return this.elements.container||(this.buildSkeleton(),this.syncInput()),this.elements.container},getInputElement:function(){return this.elements.input},_dispatchOnChange:function(){this.isDisabled()?this.syncInput():t.dispatchEvent(this.elements.input,"change")},onMouseEnter:function(){this.elements.container.addClassName("hover")},onMouseLeave:function(){this.elements.container.removeClassName("hover")},onMouseDown:function(e){this._hiddenInput&&!i.Features.touchEvents&&(t.preventDefault(e),this.focus())},onChange:function(e){this.syncInput(),this._bubbleOnChange(e)},_bubbleOnChange:function(){var e;return function(s){var i,o=this.elements.input.parentNode;if(!function(){if(void 0===e){e=!1;var s=document.createElement("div"),i=document.createElement("input");i.type="text",s.appendChild(i),s.style.display="none",document.body.appendChild(s),n.addEvent.call(s,"change",function(n){e=!0,t.stop(n)}),t.dispatchEvent(i,"change"),n.remove.call(s),n.removeEvents.call(s)}return e}())for(;o&&1===o.nodeType&&!1!==(s.event||s).returnValue;)(i=o._events&&o._events.change)&&i.handleEvent(s),o=o.parentNode}}(),onKeyDown:function(){this.syncInput()}});return u._ToggleInput=u.extend({options:{mixed:!1},name:"uwa-toggle",init:function(e){e=e||{},this._parent(e),e.mixed&&this.setMixed()},buildSkeleton:function(){this._parent(),this.elements.content.addClassName("uwa-icon")},setMixed:function(e){return this.elements.container[!1!==e?"addClassName":"removeClassName"]("mixed"),this},isChecked:function(){return this.elements.input.checked},focus:function(e){return this._parent(e),this.syncInput(),this},check:function(e){return this.elements.input.checked=!1!==e,this.syncInput(),this}}),u.Radio=u._ToggleInput.extend({name:"uwa-radio",buildInput:function(){return e.createElement("input",{type:"radio"})},onClick:function(e){this._parent(e);var t=this.elements.input;t.checked||(t.checked=!0,this._dispatchOnChange())},syncInput:function(){var e=this.elements.input,t=e.name,s=!1;function i(t){var i=t.parentNode;i&&n.hasClassName.call(i,"uwa-radio")&&n.toggleClassName.call(i,"checked",t.checked),s|=e===t}t&&Array.prototype.forEach.call(document.getElementsByName(t),i),s||i(e)}}),u.Checkbox=u._ToggleInput.extend(r,{name:"uwa-checkbox",buildInput:function(){return e.createElement("input",{type:"checkbox"})},onClick:function(e){this._parent(e),this.hasDelayed("extern-change-prevention")||this.setDelayed("extern-change-prevention",function(){this.elements.input.checked=!this.elements.input.checked,this.syncInput(),this._dispatchOnChange()},1)},onChange:function(e){this._parent(e),this.setDelayed("extern-change-prevention",function(){},1)},syncInput:function(){this.elements.container.toggleClassName("checked",this.elements.input.checked)}}),u.Select=u.extend(r,{name:"uwa-select",options:{options:[]},init:function(t){this._parent(t),e.owns(t,"options")&&this.putOptions(t.options),e.owns(t,"value")&&this.setValue(t.value)},focus:function(e){return this._parent(e),!1===e&&this.elements.dropdown.hide(),this},buildInput:function(){return e.createElement("select")},buildSkeleton:function(){var t,n=this.elements;this._parent();var s=n.container.getDocument().body;n.content.addContent([t=e.createElement("div",{class:this.getClassNames("-split"),html:[{tag:"div",class:this.getClassNames("-text")},{tag:"div",class:this.getClassNames("-button"),html:{tag:"div",class:"uwa-icon uwa-icon-only"}}]})]),n.dropdown=new a({className:this.options.className,global:!0,_root:!1,position:function(){var e=n.dropdown.getInnerElement(),t=n.container.getBoundingClientRect(),s=t.top,o=i.getSize().height-t.top-t.height,l=s>o;return e.toggleClassName("uwa-select-dropdown-top",l),e.getElement("> .uwa-select-split").inject(e,l?"bottom":"top"),e.setStyle("width",t.width),n.scroller.getContent().setStyle("height",Math.min(n.options.offsetHeight,l?s:o)),n.scroller.update(),{x:t.left,y:n.container.getOffsets().y-(l?Math.min(t.top,n.options.offsetHeight):0)}},positionOptions:{fit:"resize-max",relative:s},events:{onShow:function(){n.container&&(n.container.addClassName("dropdown-visible"),this._scrollToSelected())}.bind(this),onHide:function(){n.container&&n.container.removeClassName("dropdown-visible")},onRemoved:function(){n.container&&n.container.removeClassName("dropdown-visible")}}}),n.dropdown.getInnerElement().addClassName("uwa-select-dropdown"),n.dropdown.inject(n.content),n.options=e.createElement("div",{class:this.getClassNames("-options"),events:{mousedown:this._selectionHandler.bind(this)}}),n.scroller=new c({shadows:!1}),n.scroller.getInnerElement().addContent(n.options),n.dropdown.getInnerElement().setContent([t.cloneNode(!0),n.scroller]),this._isSingleLine()&&n.container.addClassName("single-line")},getValue:function(){return this._getSelectedOptions().map(function(e){return e.value})},setValue:function(e){var t=[];return e=s.splat(e),this._getOptions().forEach(function(n,s){-1!==e.indexOf(n.value)&&t.push(s)}),this.setSelection(t)},setSelection:function(e){return this._isMultiple()||(e=e.slice(0,1)),this._getOptions().forEach(function(t,n){t.selected=-1!==e.indexOf(n)}),this._dispatchOnChange(),this},getSelection:function(){var e=[];return this._getOptions().forEach(function(t,n){t.selected&&e.push(n)}),e},_isMultiple:function(){return this.elements.input.multiple},_isSingleLine:function(){return this.options.singleLine},_getOptions:function(){return this.elements.input.getElements("option")},_getSelectedOptions:function(){return this._getOptions().filter(function(e){return e.selected})},_dispatchOnChange:function(){this.clearDelayed("on-change-debounce"),this._parent()},_selectionHandler:function(e){t.stop(e),this._isMultiple()||(this.elements.dropdown.hide(),this.elements.container.removeClassName("hover"));var n,s,i=t.findElement(e,".option,.optgroup"),o=0,l=[],a=i.hasClassName("option"),c=!1;i.getParent().getChildren().some(function(e){if(a){if(i===e)return l.push(o),!0}else if(c){if(!e.hasClassName("option"))return!0;l.push(o)}else i===e&&(c=!0);e.hasClassName("option")&&(o+=1)}),this._isMultiple()&&(n=this.getSelection(),a?-1===(s=n.indexOf(l[0]))?n.push(l[0]):n.splice(s,1):l.some(function(e){return n.indexOf(e)<0})?l.forEach(function(e){n.indexOf(e)<0&&n.push(e)}):n=n.filter(function(e){return l.indexOf(e)<0}),l=n),this.setSelection(l)},syncInput:function(){var t=this.elements.input,s=this.elements;!this._getOptions().length||this._getSelectedOptions().length||this._isMultiple()||(this._getOptions()[0].selected=!0);var i,o,l=this._getSelectedOptions().map(n.getText.call,n.getText).join(", ")||" ";s.content.getElement(".uwa-select-text").setText(l),s.dropdown.getInnerElement().getElement(".uwa-select-text").setText(l),s.options.empty(!0).setContent((o=Array.prototype.map.call(t.getElementsByTagName("*"),function(t){var s=n.getTagName.call(t),o=e.createElement("div",{class:s+(t.selected?" selected":""),text:t.label||n.getText.call(t)||" "});return"optgroup"===s?(i&&i.addClassName("selected"),i=o):t.selected||(i=null),o}),i&&i.addClassName("selected"),o))},_scrollToSelected:function(){var e=this.elements.dropdown&&this.elements.dropdown.getInnerElement().getElement(".option.selected");e&&o.scrollToElement(e)},onClick:function(e){this._parent(e),this.elements.dropdown.show()},onKeyDown:function(e){var n=t.whichKey(e),s=!0;"space"===n?this.elements.dropdown.show():"return"===n?this.elements.dropdown.toggle():"esc"===n?this.elements.dropdown.hide():s=!1,s?t.preventDefault(e):(this._parent(e),this.setDelayed("scroll-to-selected",this._scrollToSelected,1))},putOptions:function(t,i){var o=this.elements.input;function l(e,t){var n,s=o.getElementsByTagName("*");for(n=0;n<s.length;n+=1)if(s[n][e]===t)return s[n]}return i&&n.empty.call(o,!0),s.splat(t).forEach(function(t){var s,i,a=l("value",t.value);void 0!==t.label?(a||(a=e.createElement("option")),n.set.call(a,{text:t.label,value:t.value,selected:t.selected}),t.group?((i=l("label",t.group))||(i=o.appendChild(e.createElement("optgroup",{label:t.group}))),i.appendChild(a)):o.appendChild(a)):a&&(s=a.parentNode,n.remove.call(a),s&&"optgroup"===n.getTagName.call(s)&&0===s.childNodes.length&&n.remove.call(s))}),this.syncInput(),this},removeOptions:function(e){this.putOptions(s.splat(e).map(function(e){return{value:"string"==typeof e?e:e.value}}))}}),u.File=u.extend({name:"uwa-file",buildInput:function(){return e.createElement("input",{type:"file"})},buildSkeleton:function(){this._parent(),this.options.buttonOnly?this.elements.content.addClassName("button-only"):this.elements.text=e.createElement("div",{class:this.getClassNames("-text")}),this.elements.content.addClassName(this.getClassNames("-split")).setContent([this.elements.text,e.createElement("div",{class:this.getClassNames("-button"),text:e.i18n("Browse...")})])},setValue:function(t){if(t)throw new Error("You can't set a value to a file input");var n,s=this.elements.input;s.value="",s.value&&((n=e.extendElement(e.clone(s))).inject(s,"before"),s.destroy(),this.elements.input=n,this._syncEvents(!0)),this.syncInput()},syncInput:function(){this.elements.text&&this.elements.text.setText(this.elements.input.value.replace(/^c:\\fakepath\\/i,"")||" ")}}),u.Text=u.extend(r,{name:"uwa-text",_hiddenInput:!1,options:{multiline:!1},buildInput:function(){return this.options.multiline?e.createElement("textarea"):e.createElement("input",{type:"text"})},buildSkeleton:function(){this._parent(),this.elements.input.addClassName(this.getClassNames("-text"))},onKeyDown:function(e){this._parent(e),this.setDelayed("placeholder-sync",this.syncInput,1)},onHide:function(){this._parent(),this.setDelayed("placeholder-sync",this.syncInput,1)},onShow:function(){this._parent(),this.setDelayed("placeholder-sync",this.syncInput,1)},onPostInject:function(){this.setDelayed("placeholder-sync",this.syncInput,50)},getInputElement:function(){return this.setDelayed("placeholder-sync",this.syncInput,1),this._parent()},syncInput:function(){var e=this.elements.input;i.Features.inputPlaceholder||(e.parentNode&&!this.getValue()&&e.getAttribute("placeholder")&&e.offsetHeight?this._showPlaceholder():this._hidePlaceholder())},_showPlaceholder:function(){var t,n,s=this.elements,i=s.input,o=i.getDimensions();s.placeholder||(this.setPeriodical("placeholder-sync",this.syncInput,1e3),s.placeholder=e.createElement("div",{class:this.getClassNames("-placeholder"),events:{click:this.focus.bind(this,!0)}})),o.width&&o.height?((n=i.getStyles(["font"])).height=o.innerHeight,n.width=o.innerWidth,"textarea"!==i.getTagName()&&(n.lineHeight=o.innerHeight+"px",n.whiteSpace="nowrap"),(t=i.getPosition()).x+=i.getComputedSize("marginLeft","paddingLeft","borderLeftWidth"),t.y+=i.getComputedSize("marginTop","paddingTop","borderTopWidth"),s.placeholder.set({text:i.getAttribute("placeholder"),styles:n}).setPosition(t),s.placeholder.previousSibling!==i&&s.placeholder.inject(i,"after")):this._hidePlaceholder()},_hidePlaceholder:function(){var e=this.elements.placeholder;e&&e.remove()}}),u.Password=u.Text.extend({options:{multiline:!1,attributes:{type:"password"}}}),u.Button=u.extend({name:"uwa-button",options:{className:"dark-grey"},_hiddenInput:!1,init:function(t){e.owns(t,"className")&&(t.className=t.className.replace(/\bblack\b/,"dark-grey"),/\b(?:iconl|iconr|icon-only)\b/.test(t.className)&&(t.className+=" uwa-icon"),/\b(?:dark-grey)\b/.test(t.className)&&(t.className+=" icon-separated")),this._parent(t),/\b(?:icon-only)\b/.test(this.options.className)&&this.setValue(" ")},buildInput:function(){return e.createElement("button",{type:"button"})}}),e.namespace("Controls/Input",u,e)});
define("UWA/Controls/Form",["UWA/Core","UWA/String","UWA/Utils","UWA/Event","UWA/Json","UWA/Controls/Abstract","UWA/Controls/Input"],function(e,t,n,a,l,i,s){"use strict";var c=i.extend({id:null,defaultOptions:{className:"uwa-form",fields:[],labelPreffix:":",nativeInputs:!1,darkBackground:!1},init:function(e){this._parent(e),this.id=n.random(10),this.buildSkeleton()},buildSkeleton:function(){var t,n,l,i=this.options,s=this.options.fields,c=this.fields,r=[],o=e.createElement("form",{class:i.className,id:this.id,events:{submit:function(e){a.stop(e),this.dispatchEvent("onSubmit",[e,this.getFormValues()])}.bind(this)}});for(i.nativeInputs||o.addClassName("uwa-form-uikit"),t=0,n=s.length;t<n;t++)"hidden"!==(l=s[t]).type&&(void 0===c[l.type]&&(l.type="text"),l.id="m_"+this.id+"_"+l.name,r.push(c[l.type](l,i,this)));e.createElement("fieldset",{html:r}).inject(o),this.elements.container=o},getFields:function(){var e=this.elements.container,t=n.toArray(e.getElementsByTagName("textarea")),a=n.toArray(e.getElementsByTagName("input")),l=n.toArray(e.getElementsByTagName("select"));return a.concat(l).concat(t)},getField:function(e){var t,n,a,l=this.getFields();for(t=0,n=l.length;t<n;t++)if((a=l[t]).name===e)return a},getFormValues:function(){var e,t,n={},a=this.getFields();function l(e){return e.getElements("option").filter(function(e){return e.selected}).map(function(e){return e.value})}for(e=0,t=a.length;e<t;e++){var i=a[e];switch(i.type){case"button":case"submit":break;case"password":""!==i.value&&(n[i.name]=i.value);break;case"checkbox":n[i.name]=Boolean(i.checked),"string"==typeof i.value&&(n[i.name]=String(n[i.name]));break;case"radio":i.checked&&(n[i.name]=i.value);break;default:"select"===i.getTagName()&&i.multiple?n[i.name]=l(i):n[i.name]=i.value}}return n},getFormValue:function(e){return this.getFormValues()[e]},setFormValues:function(e){var t,n,a,l,i=this.getFields();for(t=0,n=i.length;t<n;t++)if(a=i[t],e.hasOwnProperty(a.name))switch(l=e[a.name],a.type){case"password":case"button":case"submit":break;case"checkbox":a.checked=Boolean(l);break;case"radio":a.checked&&String(a.value)===l&&(a.checked=Boolean(l));break;default:a.value=l}},setFormValue:function(e,t){var n={};n[e]=t,this.setFormValues(n)},fields:{text:function(n,a,l){var i=e.createElement("input",{type:"text",id:n.id,class:n.type+" small",name:n.name,value:n.value||"",autocomplete:"off",autocorrect:"off",autocapitalize:"off"});return n.onchange&&i.addEvent("keyup",function(){this.dispatchEvent("onChange",[n.onchange,n.name,i.value])}.bind(l)),e.createElement("div",{class:"field field"+t.ucfirst(n.type),html:[{tag:"label",for:n.id,text:e.i18n((n.label||n.name)+a.labelPreffix)},{tag:"span",content:a.nativeInputs?i:new s.Text({_root:!1,element:i,className:"small"})}]})},password:function(n,a,l){var i=e.createElement("input",{type:"password",id:n.id,class:n.type,name:n.name,value:n.value||""});return n.onchange&&i.addEvent("keyup",function(){this.dispatchEvent("onChange",[n.onchange,n.name,i.value])}.bind(l)),e.createElement("div",{class:"field field"+t.ucfirst(n.type),html:[{tag:"label",for:n.id,text:e.i18n((n.label||n.name)+a.labelPreffix)},{tag:"span",content:a.nativeInputs?i:new s.Text({_root:!1,element:i,className:"small"})}]})},submit:function(n,a){var l=e.createElement("input",{id:n.id,class:n.type,type:"submit",name:n.name,value:n.value||e.i18n("Done")});return e.createElement("div",{class:"field field"+t.ucfirst(n.type),html:{tag:"span",content:a.nativeInputs?l:new s.Button({_root:!1,element:l,className:"light-grey small"})}})},button:function(n,a){var l=e.createElement("button",{id:n.id,class:n.type,name:n.name,text:n.value||e.i18n("Done")});return e.createElement("div",{class:"field field"+t.ucfirst(n.type),html:{tag:"span",content:a.nativeInputs?l:new s.Button({_root:!1,element:l,className:"light-grey small"})}})},reset:function(n,a){var l=e.createElement("button",{id:n.id,type:"reset",class:n.type,name:n.name,value:n.value||e.i18n("Done")});return e.createElement("div",{class:"field field"+t.ucfirst(n.type),html:{tag:"span",content:a.nativeInputs?l:new s.Button({_root:!1,element:l,className:"light-grey small"})}})},boolean:function(n,a,l){var i,c=n.id,r=e.createElement("div",{class:"field field"+t.ucfirst(n.type)}),o="string"!=typeof n.value||"true",u=n.value&&(!0===n.value||"true"===n.value);return e.createElement("label",{for:c,text:e.i18n(n.label||n.name)}).inject(r),i=e.createElement("input",{id:c,value:o,type:"checkbox",class:n.type+" "+(u?"checked":"unchecked"),name:n.name}),u&&(i.setAttribute("checked","checked"),i.defaultChecked=!0),i.addEvent("change",function(){var e=i.checked;i.addClassName(e?"checked":"unchecked"),i.removeClassName(e?"unchecked":"checked"),n.onchange&&this.dispatchEvent("onChange",[n.onchange,n.name,e?"true":"false"])}.bind(l)),e.createElement("span",{html:a.nativeInputs?i:new s.Checkbox({_root:!1,element:i,className:a.darkBackground?"green":""})}).inject(r),r},textarea:function(n,a,l){var i=e.createElement("textarea",{id:n.id,class:n.type+" small",name:n.name,text:n.value||""});return n.onchange&&i.addEvent("keyup",function(){this.dispatchEvent("onChange",[n.onchange,n.name,i.value])}.bind(l)),e.createElement("div",{class:"field field"+t.ucfirst(n.type),html:[{tag:"label",for:n.id,text:e.i18n((n.label||n.name)+a.labelPreffix)},a.nativeInputs?i:new s.Text({_root:!1,element:i})]})},range:function(n,a,l){var i,c,r,o,u=n.id,m=e.createElement("div",{class:"field field"+t.ucfirst(n.type)});if(e.createElement("label",{for:u,text:e.i18n((n.label||n.name)+a.labelPreffix)}).inject(m),r=e.createElement("span").inject(m),o=e.createElement("select",{id:"m_"+l.id+"_"+n.name,class:"range",name:n.name}).inject(r),n.step=parseInt(n.step,10),n.max=parseInt(n.max,10),n.min=parseInt(n.min,10),n.step>0)for(i=n.min;i<=n.max;i+=n.step)c=e.createElement("option",{value:i,text:String(i)}),n.value&&parseInt(n.value,10)===i&&(c.setAttribute("selected","selected"),c.selected=!0),o.appendChild(c);return n.onchange&&o.addEvent("change",function(){this.dispatchEvent("onChange",[n.onchange,n.name,o.value])}.bind(l)),a.nativeInputs||new s.Select({_root:!1,element:o,className:"small"}),m},list:function(a,l,i){var c,r,o,u,m,d,f="m_"+i.id+"_"+a.name,h=e.createElement("div",{class:"field field"+t.ucfirst(a.type)});if(e.createElement("label",{for:f,text:e.i18n((a.label||a.name)+l.labelPreffix)}).inject(h),m=e.createElement("span").inject(h),d=e.createElement("select",{id:"m_"+i.id+"_"+a.name,class:"list",name:a.name,multiple:Boolean(a.multiple)}).inject(m),e.is(a.options,"array")&&a.options.length>0){var p=n.splat(a.value).map(function(e){return String(e)});for(c=0,r=a.options.length;c<r;c++)(o=a.options[c]).label=o.label||o.value,u=e.createElement("option",{text:e.i18n(o.label),value:o.value}).inject(d),p.indexOf(String(o.value))>=0&&(u.setAttribute("selected","selected"),u.selected=!0);a.onchange&&d.addEvent("change",function(){this.dispatchEvent("onChange",[a.onchange,a.name,d.value])}.bind(i))}else h.hide();return l.nativeInputs||new s.Select({_root:!1,element:d,className:"small"}),h},checklist:function(a,i,c){var r,o,u,m,d,f=[],h="m_"+c.id+"_"+a.name,p=e.createElement("div",{class:"field field"+t.ucfirst(a.type)});if(e.createElement("label",{for:h,text:e.i18n((a.label||a.name)+i.labelPreffix)}).inject(p),m=e.createElement("span",{class:a.type}).inject(p),d=e.createElement("input",{id:"m_"+c.id+"_"+a.name,name:a.name,type:"hidden",value:e.is(a.value,"array")?l.encode(a.value):a.value}).inject(m),e.is(a.options,"array")&&a.options.length>0){var v=e.is(a.value,"array")?a.value:l.decode(a.value),g=n.splat(v).map(function(e){return String(e)});for(r=0,o=a.options.length;r<o;r++){(u=a.options[r]).label=u.label||u.value;var b=g.indexOf(String(u.value))>=0,E=e.createElement("p").inject(m),y=e.createElement("input",{value:u.value,type:"checkbox",name:u.value,checked:b});f.push(y),y.addEvent("change",function(){var e=[];f.forEach(function(t){t.checked&&e.push(t.value)}),d.value=l.encode(e),a.onchange&&this.dispatchEvent("onChange",[a.onchange,a.name,d.value])}.bind(c)),e.createElement("span",{html:i.nativeInputs?y:new s.Checkbox({_root:!1,className:i.darkBackground?"green":"",element:y})}).inject(E),e.createElement("label",{text:e.i18n(u.label)}).inject(E)}}else p.hide();return p},html:function(n){return e.createElement("div",{class:"field field"+t.ucfirst(n.type),html:{tag:"div",html:n.html}})},img:function(n){var a=e.i18n(n.label||n.name)||"";return e.createElement("div",{class:"field field"+t.ucfirst(n.type),html:{tag:"img",src:n.src,height:n.height||"auto",width:n.width||"100%",alt:a,title:a}})}}});return e.namespace("Controls/Form",c,e)});
define("UWA/Widget",["UWA/Core","UWA/String","UWA/Array","UWA/Class","UWA/Class/Options","UWA/Class/Timed","UWA/Class/Events","UWA/Class/Debug","UWA/Utils","UWA/Utils/Client","UWA/Data","UWA/Element"],function(e,t,n,i,r,s,a,o,h,u,l,d){"use strict";function c(e){if(!Array.isArray(e))throw new Error(e+" should be an array");e.forEach(function(e){if("string"!=typeof e)throw new Error(e+" should be a string")})}function f(e,t){if(e){if(e.multiple||"checklist"===e.type)try{t=function(e){if(!e)return[];var t;if(Array.isArray(e))t=e;else try{t=JSON.parse(e)}catch(t){throw new Error("While parsing JSON value `"+e+"`: "+t)}return c(t),t}(t)}catch(t){throw new Error("While decoding value for preference "+e.name+": "+t)}"boolean"===e.type&&"boolean"!=typeof t&&void 0!==t&&(t="false"!==t&&Boolean(t))}return t}var m,p=i.extend(r,s,a,o,{init:function(){var e=u.Locale;this.id=null,this.environment=null,this.launched=!1,this.title=null,this.icon=null,this.counter=0,this.counterType=null,this.metas={},this.preferences=[],this.defaultData=Object.create(null),this.data={},this.plugins=[],this.events={},this.menus=[],this.elements={},this.body=null,this.lang=e.lang,this.locale=e.locale,this.dir=e.dir,this.readOnly=!1,this.isEdit=!1},launch:function(e,t){var n=this;return n.launched=!1,void 0!==t&&(n.readOnly=Boolean(t)),n.initPreferences(),n.initPlugins(),n.setValues(e),n.dispatchEvent("onInitConfig",{metas:n.metas,plugins:n.plugins,preferences:n.getPreferences()}),n.dispatchEvent("beforeLoad"),n.addEventOnce("onLoad",function(){n.launched=!0},n,1),n.dispatchEvent("onLoad"),n.launched&&n.dispatchEvent("afterLoad"),n.launched},destroy:function(){var e,t=this.elements;for(e in this.clearDelayed(),this.clearPeriodical(),t)t.hasOwnProperty(e)&&t[e].destroy();this.removeEvent(),this.launched=!1},setOptions:function(n){var i,r;for(i in n)r="set"+t.capitalize(i),e.is(this[r],"function")&&this[r](n[i]);return this._parent(n)},setAutoRefresh:function(e){(e=parseInt(e,10))&&e>0?this.setPeriodical("autoRefresh",this.dispatchEvent.bind(this,"onRefresh"),1e3*e*60):this.clearPeriodical("autoRefresh"),this.metas.autoRefresh=e},setCounter:function(t,n){(this.counter!==t||e.is(n)&&this.counterType!==n)&&(this.counter=t,this.counterType=n,this.dispatchEvent("onUpdateCounter",[t,n]))},getTitle:function(){return e.is(this.title,"string")?t.stripTags(this.title):""},setTitle:function(t,n){return(e.is(t,"string")||n&&this._titleUrl!==n)&&(this.title=t,this._titleUrl=n,this.dispatchEvent("onUpdateTitle",[t,n])),this.title},setIcon:function(t,n){return t&&e.is(t,"string")&&(n&&(t=l.proxifyUrl(t,{proxy:"icon"})),this.icon!==t&&(this.icon=t,this.dispatchEvent("onUpdateIcon",[t]))),this.icon},setMenu:function(t){var n,i,r,s=this.environment,a=t.name.split("/"),o=a[0];if(a.length>2)throw new Error("Adding more than one submenu level is not supported by setMenu");(r=this.getMenu(t.name))?e.extend(r,t):(a.length>1?((n=this.getMenu(o))||(n={label:o},this.menus.push(n)),n.items||(n.items=[]),i=n.items):i=this.menus,i.push(t)),this.setDelayed("onUpdateMenu",function(){s.dispatchEvent("onUpdateMenu",[this.menus])},20)},getMenu:function(t){var i,r;return e.is(t,"string")&&(r=t.split("/"),(i=n.detect(this.menus,function(e){return e.name===r[0]}))&&r.length>1&&(i=i.items&&n.detect(i.items,function(e){return e.name===t}))),i},removeMenu:function(e){var t,n,i,r;for(r=function(t){return t.name!==e},t=0,n=this.menus.length;t<n;t++){if((i=this.menus[t]).name===e){this.menus.remove(i);break}i.items&&(i.items=i.items.filter(r))}},setDir:function(e){var t=this.dir,n=this.elements.wrapper;return e="rtl"===e?"rtl":"ltr",n&&t!==e&&(n.setAttribute("dir",e),n.addClassName(e),n.removeClassName(t)),this.dir=e,e},setMetas:function(t){return e.extend(this.metas,t),e.is(t.debugMode)&&(this.setDebugMode(t.debugMode),this.environment&&this.environment.setDebugMode(t.debugMode)),e.is(t.autoRefresh)&&this.setAutoRefresh(t.autoRefresh),this.metas},setBody:function(e){if(!this.body)throw new Error("Widget.body is not yet available");this.body.setContent(e)},addBody:function(e){this.body.addContent(e)},getElements:function(e){return this.body.getElements(e)},getElement:function(e){return this.body.getElement(e)},createElement:function(t,n){return e.createElement(t,n)},setStyle:function(e){var t=this.id?"#m_"+this.id:".moduleWrapper";this.id&&this.elements.wrapper.setAttribute("id","m_"+this.id),h.setCss(!1,e,t,this.getUrl())},mutate:function(e,t){var n=this.environment;if(!e)throw new Error("Missing or empty first param on widget.mutate");if(!n||!n.mutate)throw new Error("Current Environment do not support widget.mutate");n.mutate(e,t)},getUrl:function(){var e=window.location.href;return this.uwaUrl?this.uwaUrl:h.getQueryString(e,"uwaUrl",e)},addStar:function(e){var t=this.environment;t&&t.addStar&&t.addStar(e)},getViewportDimensions:function(){var e,t,n=this.elements,i=n.body,r=d.getDimensions,s=d.isInjected,a=d.getComputedSize,o=u.getSize(),h=r.call(n.wrapper),l=r.call(i),c=o.height,f=h.width;["header","footer"].forEach(function(t){(e=n[t])&&s.call(e)&&(c-=r.call(e).outerHeight)}),e=i,t=n.wrapper.parentNode;do{e!==n.wrapper?f-=a.call(e,"innerWidth","outerWidth"):f-=a.call(e,"innerWidth"),c-=a.call(e,"innerHeight","outerHeight"),e=e.parentNode}while(e&&e!==t);return l.maxHeight>0&&c>l.maxHeight?c=l.maxHeight:l.minHeight>0&&c<l.minHeight&&(c=l.minHeight),{height:c<0?240+c:c,width:f<0?320+f:f}},setPlugins:function(e){this.plugins=e},initPlugins:function(){var t,n,i,r=e.clone(this.plugins);for(t=0,n=r.length;t<n;t++)i=r[t],e.Plugins[i.name]&&(i.instance=new e.Plugins[i.name](this,i.options))},initPreferences:function(){this.setPreferences(this.preferences)},hasPreferences:function(){var e=this.preferences;return!this.readOnly&&e.length>0&&e.some(function(e){return"hidden"!==e.type})},_getRawPreference:function(e){return n.detect(this.preferences,function(t){return t.name===e})},getPreference:function(t){var n=this._getRawPreference(t);return n&&((n=e.clone(n)).value=this.getValue(t)),n},hasPreference:function(e){return this.preferences.some(function(t){return t.name===e})},addPreference:function(){var t=["hidden","text","list","checklist","range","password","boolean"];return function(n){var i,r=-1,s=this.preferences;(function(e){return e.name&&e.type&&-1!==t.indexOf(e.type)})(n)&&(i=void 0!==(n=e.clone(n)).defaultValue,n.multiple&&"boolean"!=typeof n.multiple&&(n.multiple="true"===n.multiple),i&&(n.defaultValue=f(n,n.defaultValue)),s.forEach(function(e,t){n.name===e.name&&(r=t)}),n.label||(n.label=n.name),-1!==r?s[r]=n:s.push(n),this.defaultData[n.name]=n.defaultValue,this.launched&&this.dispatchEvent("onUpdatePreferences",[this.getPreferences()]))}}(),setPreferences:function(e){var t,n;for(this.preferences=[],this.defaultData={},this.launched&&0===e.length&&this.dispatchEvent("onUpdatePreferences",[this.getPreferences()]),t=0,n=e.length;t<n;t++)this.addPreference(e[t])},mergePreferences:function(e){var t,n;for(t=0,n=e.length;t<n;t++)this.hasPreference(e[t].name)||this.addPreference(e[t])},getPreferences:function(){var t,n,i,r,s,a,o=e.clone(this.preferences);for(t=0,n=o.length;t<n;t++)if((s=o[t]).value=this.getValue(s.name),s.label=e.i18n(s.label),e.is(s.options,"array"))for(i=0,r=s.options.length;i<r;i++)(a=s.options[i]).label=e.i18n(a.label);return o},getValue:function(t){var n=this.environment,i=this.data[t];return!e.is(i)&&n&&n.getData&&(i=f(this._getRawPreference(t),n.getData(t))),e.is(i)||(i=this.defaultData[t]),e.is(i)?this.data[t]=i:(i=void 0,delete this.data[t]),i},getInt:function(e){var t=this.getValue(e);return t="true"===t||!0===t?1:parseInt(t,10),isNaN(t)?0:t},getBool:(m=[1,"1","true",!0],function(e){return-1!==m.indexOf(this.getValue(e))}),setValue:function(t,n){var i=this.environment,r=this._getRawPreference(t),s=!0;return n=f(r,n),e.equals(this.data[t],n)||(e.is(n)?(n=e.clone(n),this.data[t]=n,i&&i.setData&&i.setData(t,function(e,t){return e&&(e.multiple||"checklist"===e.type)&&(c(t),t=JSON.stringify(t)),t}(r,n),!!r&&e.equals(r.defaultValue,n))):(this.data.hasOwnProperty(t)?delete this.data[t]:s=!1,i&&i.deleteData?i.deleteData(t):i&&i.setData&&i.setData(t,void 0)),s&&this.dispatchEvent("onUpdateValue",[t,n])),n},setValues:function(e){var t;for(t in e)e.hasOwnProperty(t)&&this.setValue(t,e[t])},deleteValue:function(e){return this.setValue(e)},toggleEdit:function(){this.dispatchEvent(this.isEdit?"endEdit":"onEdit")},dispatchEvent:function(e,t,n,i){var r=this.environment,s=!i&&r||"onLoad"===e||this.launched;return!i&&r?r.dispatchEvent(e,t,n):s&&this._parent(e,t,n),this},addEvent:function(e,t,n,i){var r=this,s="onLoad"===e&&r.launched;return r._parent(e,t,n,i),s&&(r.addEventOnce("_onLoadImmediate",t,n,i),this.setImmediate("_onLoadImmediate",function(){r.dispatchEvent("_onLoadImmediate")})),r},addEventOnce:function(e,t,n,i){var r=this;return"onLoad"===e&&r.launched?(r.addEventOnce("_onLoadImmediate",t,n,i),this.setImmediate("_onLoadImmediate",function(){r.dispatchEvent("_onLoadImmediate")})):r._parent(e,t,n,i),r},requestView:function(t){return e.is(t,"string")&&(t={type:t}),this.dispatchEvent("onViewRequest",[t]),this},getView:function(){return this._view||{type:"windowed"}},getAvailableViews:function(){var e=this.metas.availableViews||"";return n.invoke(e.split(";"),"trim").filter(function(e){return e}).map(function(e){var t,n=e.match(/\S*/)[0],i=e.slice(n.length).trim();if(i)try{t=JSON.parse(i)}catch(e){this.log("Failed to parse availableViews options")}return t||(t={}),t.type=n,t},this)},onEdit:function(){this.isEdit=!0},endEdit:function(){this.isEdit=!1}});return e.namespace("Widget",p,e)});
define("UWA/Controls/WidgetPopupMenu",["UWA/Core","UWA/Element","UWA/Event","UWA/Utils","UWA/Controls/DropDown"],function(t,e,n,i,s){"use strict";var a=s.extend({name:"uwa-widget-popup-menu",init:function(t){this._parent(),this.env=t,this.items=null},setTarget:function(t){return this.target=t,this},onClick:function(t){this._parent(t);var e=n.findElement(t,"li"),i=this.env.widget.getMenu(e.getAttribute("data-name"));i&&this.env.dispatchEvent("onMenuExecute",[i])},onClickOutside:function(t){n.getElement(t)!==this.target&&this.hide()},setPosition:function(){var t,n=this.env.html.moduleFrame||this.env.html.wrapper,i=e.getOffsets.call(n),s=e.getSize.call(n),a=e.getOffsets.call(this.target),o=e.getSize.call(this.target);return{x:a.x,y:a.y+o.height},t={boundary:{x:0,y:a.y+o.height,width:i.x+s.width,height:1/0}},this._parent(a,t)},getInnerElement:function(){return this.getContent(),this.elements.inner},getContent:function(){var e=this.elements;return e.inner||this._parent().setContent(e.inner=t.createElement("menu",{type:"popup"})),e.container},setItems:function(t){return this.items=t,this},toggle:function(){this.getInnerElement().empty(),this.items.forEach(this.addItem,this),this.setPosition(),this._parent()},onShow:function(){this.target.addClassName("active"),this._parent()},onHide:function(){this.target.removeClassName("active"),this._parent()},addItem:function(e){var n,s;if(!1!==(t.is(e.visible,"function")?e.visible():!1!==e.visible))return n=t.createElement("li",{class:this.getClassNames("-item"),"data-name":e.name}),e.icon&&(s=t.createElement("span",{class:"uwa-icon uwa-icon-only"}),1===this._getUtf8StringLength(e.icon)?(s.set("data-icon",e.icon),s.addClassName("uwa-icon-unicode")):i.isAbsoluteUrl(e.icon)?s.adopt(t.createElement("img",{src:e.icon,width:16,height:16})):s.addClassName(e.icon),s.inject(n)),e.label&&t.createElement("span",{text:e.label}).inject(n),(t.is(e.disabled,"function")?e.disabled():!!e.disabled)&&n.addClassName("disabled"),n.inject(this.getInnerElement())},_getUtf8StringLength:function(t){var e=encodeURIComponent(t).match(/%[89ABab]/g);return t.length+(e?e.length:0)}});return t.namespace("Controls/WidgetPopupMenu",a,t)});
define("UWA/Utils/InterCom",["UWA/Core","UWA/String","UWA/Utils","UWA/Class","UWA/Dispatcher","UWA/Class/Events","UWA/Class/Options","UWA/Class/Timed","UWA/Class/Debug","UWA/Json"],function(e,t,s,n,r,i,o,a,c,u){"use strict";function d(e,t){var s,n,r,i;for(s=0,n=e.length;s<n;s++)for(r=0,i=t.length;r<i;r++)if(t[r]===e[s])return!0;return!1}function v(e){return Boolean(e.UWA&&e.UWA.Utils&&e.UWA.Utils.InterCom)&&!e.UWA.Utils.InterCom._listener&&(e.UWA.Utils.InterCom._listener=new i),e.UWA.Utils.InterCom._listener}var h,l=e.getGlobal();return(h={getAdapter:function(e){var t,n,r,i=h.Adapters,o=e?s.splat(e):Object.keys(i);for(t=0,n=o.length;t<n&&!r;t++){if(e=o[t],!i.hasOwnProperty(e))throw new Error('Unable to get InterCom Adapter with name "'+e+'"');if(i[e].isAvailable(r)){r=i[e];break}}if(!r)throw new Error("Unable to get InterCom Adapter");return r}}).Adapters={PostMessage:function(){var e,n="uwa-intercom";function i(t){var s;try{s="string"==typeof t.data&&"{"===t.data[0]&&JSON.parse(t.data)}catch(e){}s&&s.type===n&&e.dispatch([s.payload,{origin:t.origin,source:t.source}])}return{isAvailable:function(){return l.postMessage&&l.location&&l.location.protocol&&t.contains(l.location.protocol,"http")},removeListener:function(t){e&&(e.remove(t),0===e.getNumListeners()&&(e.dispose(),e=void 0,l.addEventListener?l.removeEventListener("message",i,!1):l.attachEvent&&l.detachEvent("onmessage",i)))},addListener:function(t){e||(e=e||new r,l.addEventListener?l.addEventListener("message",i,!1):l.attachEvent&&l.attachEvent("onmessage",i)),e.add(t)},dispatchEvent:function(e,t,r){var i;if(t||(t=(i=l.parent).postMessage?i:i.document.postMessage?i.document:void 0),r=r&&"*"!==r?s.buildUrl(l.location,r):"*",t&&t.postMessage){var o={type:n,payload:e};t.postMessage(JSON.stringify(o),r)}}}}(),FrameCallback:function(){var e,t=0,n=[],r=!0,i=l.document;function o(){r&&i.body&&n.length>0&&i.body.appendChild(n.shift()),n.length>0&&setTimeout(o,10)}return{isAvailable:function(){return e=v(l),Boolean(e)},removeListener:function(t){e.removeEvent("message",t)},addListener:function(t){e.addEvent("message",t)},dispatchEvent:function(e,a,c){!function(e){try{return e===l||e.location.host===l.location.host&&e.location.protocol===l.location.protocol}catch(e){}}(a)?function(e,a,c){var d,v,h=l.location.toString(),g=s.parseUrl(c),p=g.protocol+"://"+g.domain+"/intercom.html",f={info:e,origin:h};d="#"+Date.now()+t+++"&"+u.encode(f),(v=i.createElement("iframe")).setAttribute("src",p+d),v.style.position="absolute",v.style.top="-2000px",v.style.left="0px",v.onload=function(){r=!0,v.parentNode.removeChild(v)},n.push(v),setTimeout(o,10)}(e,0,c):function(e,t){var s=v(t);setTimeout(function(){s.dispatchEvent("message",[e,{origin:l.location.toString(),source:l}])})}(e,a)}}}()},h.Server=n.extend(o,c,{id:null,uuid:null,sockets:null,listeners:null,defaultOptions:{adapter:null,autoconnect:!0},init:function(e,t){this.setServerId(e),this.sockets={},this.listeners=new i,this.setOptions(t),this.options.autoconnect&&this.connect()},setServerId:function(e){var t=h.Server.Instances=h.Server.Instances||{};return this.uuid=this.uuid||s.getUUID(),t[e=e||this.uuid]&&(t[e].disconnect(),delete t[e]),this.id=e,t[e]=this,this},connect:function(){return this.handleEvent=this.handleEvent.bind(this),this.adapter=h.getAdapter(this.options.adapter),this.adapter.addListener(this.handleEvent),this},disconnect:function(){var e=this;return e.adapter&&(Object.keys(e.sockets).forEach(function(t){e.unsubscribeSocket(t)}),e.adapter.removeListener(e.handleEvent)),e},handleEvent:function(e,t){var s,n,r,i=this.id,o=this.sockets,a=Object.keys(o);n=(s=t&&t.source&&t.origin&&e.event&&e.target&&e.origin&&e.target.servers&&Array.isArray(e.target.servers)&&e.target.sockets&&Array.isArray(e.target.sockets))&&o[e.origin.socket]&&o[e.origin.socket].uuid===e.uuid,r=s&&0===e.target.sockets.length&&-1!==e.target.servers.indexOf(i),s?r?(this.log('SERVER: server "'+i+'" accept message for event "'+e.event+'"'),"subscribe"===e.event?n||this.subscribeSocket(e.origin.socket,t.source,t.origin,e.uuid):n&&("unSubscribe"===e.event?this.unsubscribeSocket(e.origin.socket):this.dispatchEvent(e.event,e.data,e.origin.socket,e.target.sockets))):n&&d(e.target.sockets,a)&&d([e.origin.socket],a)?(this.log('SERVER PREDISPATCH: server "'+i+'" dispatch event "'+e.event+'" from "'+e.origin.socket+'"'),this.dispatchEvent(e.event,e.data,e.origin.socket,e.target.sockets)):this.log('SERVER: server "'+i+'" refuse message for event "'+e.event+'"'):this.log('SERVER: server "'+i+'" refuse invalid message for event "'+e.event+'"')},subscribeSocket:function(e,t,s,n){var r=this.id;return this.log('SERVER: server "'+r+'" register new socket "'+e+'"'),this.sockets[e]={source:t,origin:s,uuid:n},this.dispatchEvent("subscribe",{},void 0,e),this},unsubscribeSocket:function(e){var t=this.id;return this.sockets[e]&&(this.log('SERVER: server "'+t+'" unregister socket "'+e+'"'),this.dispatchEvent("unSubscribe",{},void 0,e),delete this.sockets[e]),this},addListener:function(e,t){return this.listeners.addEvent(e,t),this},removeListener:function(e,t){return this.listeners.removeEvent(e,t),this},dispatchEvent:function(e,t,n,r){var i=this,o=i.id,a=i.sockets,c=i.adapter,u={event:e,data:t,target:{sockets:r},origin:{socket:n,server:o},uuid:i.uuid};return r&&r.length?r=s.splat(r):-1!==(r=Object.keys(i.sockets)).indexOf(n)&&r.splice(r.indexOf(n),1),c||(i.connect(),c=i.adapter),0===r.length?i.log('SERVER: server "'+o+'" has no target socket for dispatchEvent "'+e+'"'):r.forEach(function(s){var r=a[s],u={event:e,data:t,target:{sockets:[s]},origin:{socket:n,server:o},uuid:i.uuid};i.log('SERVER: server "'+o+'" dispatchEvent "'+u.event+'" to "'+s+'"');try{c.dispatchEvent(u,r.source,r.origin)}catch(e){l.console&&l.console.error('InterCom server "'+o+'": error while dispatching to socket '+s+": "+e+"\nDeleting socket"),delete a[s]}}),i.listeners.dispatchEvent(e,[t,u]),i}}),h.Socket=n.extend(o,c,{id:null,uuid:null,servers:null,listeners:null,defaultOptions:{adapter:null,autoconnect:!1},init:function(e,t){this.setSocketId(e),this.servers={},this.listeners=new i,this.setOptions(t)},setSocketId:function(e){var t=h.Socket.Instances=h.Socket.Instances||{};return this.uuid=this.uuid||s.getUUID(),t[e=e||this.uuid]&&(t[e].disconnect(),delete t[e]),this.id=e,t[e]=this,this},connect:function(){return this.handleEvent=this.handleEvent.bind(this),this.adapter=h.getAdapter(this.options.adapter),this.adapter.addListener(this.handleEvent),this},disconnect:function(){var e=this;return e.adapter&&(Object.keys(e.servers).forEach(function(t){e.unsubscribeServer(t)}),e.adapter.removeListener(e.handleEvent)),e},handleEvent:function(e,t){var s,n,r,i,o=this,a=o.id,c=o.servers;n=(r=t&&t.source&&t.origin&&e&&e.event&&e.target&&e.origin&&e.origin.server&&c[e.origin.server]&&e.target.sockets&&Array.isArray(e.target.sockets))&&c[e.origin.server]&&c[e.origin.server].uuid===e.uuid,i=r&&0!==e.target.sockets.length&&-1!==e.target.sockets.indexOf(a),r?i?(s=o.servers[e.origin.server],o.log('SOCKET: socket "'+a+'" accept message for event "'+e.event+'"'),"subscribe"===e.event?(n||(s.waiting=!1,s.uuid=e.uuid,s.queue.length&&(s.queue.forEach(function(e){o.adapter.dispatchEvent(e,s.source,s.origin)}),o.log('SOCKET: socket dispatch "'+s.queue.length+'" events in the queue for serverId "'+e.origin.server+'".'),s.queue=[])),o.listeners.dispatchEvent(e.event,[e.data,e])):n?"unSubscribe"===e.event?delete o.servers[e.origin.server]:o.listeners.dispatchEvent(e.event,[e.data,e]):o.log('SOCKET: socket "'+a+'" refuse invalid uuid for event "'+e.event+'"')):o.log('SOCKET: socket "'+a+'" refuse message for event "'+e.event+'"'):o.log('SOCKET: socket "'+a+'" refuse invalid message for event "'+e.event+'"')},subscribeServer:function(e,t,s){return t=t||l.parent,s=s||l.location.toString(),this.servers[e]={waiting:!0,queue:[],source:t,origin:s},this.dispatchEvent("subscribe",void 0,void 0,e),this},unsubscribeServer:function(e){var t=this.id;return this.servers[e]&&(this.log('SOCKET: socket "'+t+'" unregister server "'+e+'"'),this.dispatchEvent("unSubscribe",{},void 0,e),delete this.servers[e]),this},addListener:function(e,t){return this.listeners.addEvent(e,t),this},removeListener:function(e,t){return this.listeners.removeEvent(e,t),this},dispatchEvent:function(e,t,n,r){var i=this,o=i.id,a=i.servers,c=i.adapter;return r=r&&r.length?s.splat(r):Object.keys(i.servers),n=s.splat(n),c||(i.connect(),c=i.adapter),t=u.prune(t),r.forEach(function(s){var r=a[s],u={event:e,data:t,target:{servers:[s],sockets:n},origin:{socket:o},uuid:i.uuid};0===r.queue.length&&!r.waiting||"subscribe"===e||"unSubscribe"===e?(i.log('SOCKET: socket "'+o+'" dispatch event "'+e+'"'),c.dispatchEvent(u,r.source,r.origin)):(i.log('SOCKET: socket "'+o+'" queue event "'+e+'" for serverId "'+s+'"'),r.queue.push(u))}),i}}),e.namespace("Utils/InterCom",h,e)});
define("UWA/Embedded",["UWA/Core","UWA/String","UWA/Class","UWA/Class/Options","UWA/Class/Debug","UWA/Class/Events","UWA/Utils","UWA/Utils/InterCom"],function(e,t,i,n,s,o,r,a){"use strict";function d(e,t){var i;for(i in t)t.hasOwnProperty(i)&&(e.style[i]=t[i])}function l(e,t){var i,n;for(n in t)t.hasOwnProperty(n)&&(i=t[n],"styles"===n?d(e,i):"html"===n?e.innerHTML=i:"text"===n?(e.innerHTML="",e.appendChild(document.createTextNode(i))):e.setAttribute(n,i))}function h(e,t,i){var n=document.createElement(e);return t&&l(n,t),i&&i.appendChild(n),n}function c(e){var t;if("object"!=typeof e)return!1;for(t in e)if(e.hasOwnProperty(t))return!1;return!0}function u(e){return"boolean"==typeof e?!1===e?"0":"1":r.encodeUrl(e)}var p=i.extend(n,s,o,{url:"",id:null,data:null,version:e.version,elements:null,preferences:null,disableRemote:!0,defaultOptions:{container:null,className:"module",title:null,themeUrl:null,color:"white",height:"auto",width:"100%",maxHeight:!1,bookmarklet:!1,lang:null,id:null,readOnly:!1,data:{},buildHeader:!1,displayHeader:!0,displayFooter:!0,displayScroller:!1,displayEdit:!0,cache:null,useAsyncFrame:!1,useAppCache:!1,offlineMode:!1,autoLaunch:!0,subDomain:!1,subDomainPattern:"{id}.widget.",remoteName:"uwa.embedded",sandbox:!1,exposition:e.hosts.exposition,uwa:e.hosts.uwa},socket:null,init:function(e,t){this.url=e,this.data={},this.elements={},this.preferences=[],this._remoteQueue=[],this.startTime=(new Date).getTime(),this.setOptions(t);var i,n,s,o=typeof(t=this.options).container;if("string"===o?this.container=document.getElementById(t.container):"object"===o&&null!==this.options.container?this.container=t.container:(s=document.getElementById("UWA_ASYNC"),this.container=h("div",{id:this.id,class:t.className}),s?s.parentNode.insertBefore(this.container,s.nextSibling):(n=(i=document.getElementsByTagName("script"))[i.length-1]).parentNode.insertBefore(this.container,n)),p.Instances[this.id]=this,!this.container)throw new Error("UWA.Embedded is unable to get container element with container "+this.container+".");if("string"!=typeof this.url)throw new Error("UWA.Embedded expect url defined has first param");this.log('Init new instance with container id "'+this.id+'" and widget url "'+this.url+'"'),this.render()},destroy:function(){},setOptions:function(e){return this._parent(e),(e=this.options).title&&(e.buildHeader=!0),e.buildHeader&&(e.displayHeader=!1),this.data=e.data||{},!e.id&&this.id||(this.id=e.id||this.generateId()),this},generateId:function(){var e;do{e="uwa-"+r.getCheckSum(this.url)+"-"+r.random(1,1e5)}while(document.getElementById(e)&&null!==p.Instances[e]);return e},render:function(){var t,i={},n=this.options,s=this.container,o=navigator.userAgent.toLowerCase().match(/ip(?:ad|od|hone)/);i.wrapper=h("div",{class:"moduleWrapper"}),n.buildHeader&&(i.header=h("div",{class:"moduleHeader",styles:{position:"relative",overflow:"hidden",height:"23px",padding:"5px 5px 0 5px"}},i.wrapper),i.iconContainer=h("span",{styles:{padding:"0 5px 0 0"}},i.header),i.icon=h("img",{src:n.uwa+e.paths.img+"icon.png",class:"moduleIcon",height:16,width:16,styles:{border:"none",height:16,width:16}},i.iconContainer),i.title=h("span",{text:n.title||"Loading...",class:"moduleTitle",styles:{font:'bold 11px/20px "Lucida Grande",Tahoma,Helvetica,Arial,sans-serif',verticalAlign:"top"}},i.header)),i.body=h("div",{class:"moduleContent"},i.wrapper),t={id:"frame-"+this.id,frameBorder:0,width:"100%",scrolling:n.maxHeight||"auto"!==n.height?"auto":"no"},n.sandbox&&(t.sandbox="allow-same-origin allow-forms allow-scripts allow-popups"),i.iframe=h("iframe",t,i.body),d(i.iframe,{display:"block"}),n.bookmarklet&&(n.displayScroller=!0,n.height="100%",n.width="320px",d(i.wrapper,{position:"fixed",top:0,right:0,height:n.height,width:n.width,"z-index":99999998})),"auto"!==n.height&&(i.iframe.height=n.height),o&&n.displayScroller&&(i.iframe.scrolling="no"),this.elements=i,s.innerHTML="",s.appendChild(i.wrapper),n.useAsyncFrame?this.renderIframeAsync():this.renderIframe(),this.setChromeColor(n.color),this.initRemote()},renderIframe:function(){var e=this.elements.iframe,t=this.getIframeUrl();e.previousIframeUrl&&e.previousIframeUrl===t||(e.previousIframeUrl=t,e.src=t)},renderIframeAsync:function(){var t,i=JSON.stringify,n=this.options,s=this.elements.iframe.contentWindow.document,o=n.exposition+"/widget/amd/js?uwaUrl="+u(this.url),r={id:this.id,widgetDomain:window.location.toString().replace(/#.*$/,"")};n.cache&&(o+="&cache="+u(n.cache)),t=["<!DOCTYPE html>","<html>","<head>",'<meta charset="UTF-8" />','<script type="text/javascript">',"   var UWA = {hosts:"+i(e.hosts)+"},",'       curl = {apiName: "require"};',"<\/script>",'<script type="text/javascript" src="'+n.uwa+"/lib/vendors/curl.js?v="+this.version+'"><\/script>','<script type="text/javascript" src="'+o+"&v="+this.version+'"><\/script>',"</head>","<body>",'<script type="text/javascript">','   define("'+this.id+'", ["'+this.url+'"], function (widget) {',"       UWA.extend(widget, "+i(r)+");","   });","<\/script>","</body>","</html>"],s.open(),s.write(t.join("\n")),s.close()},getIframeUrl:function(){var e,t,i=[],n=this.options,s=this.data,o={uwaUrl:this.url,id:this.id,cache:n.cache,header:n.displayHeader,footer:n.displayFooter,scroller:n.displayScroller,displayEdit:n.displayEdit,autoLaunch:n.autoLaunch&&!n.offlineMode,useAppCache:n.useAppCache,offlineMode:n.offlineMode,chromeColor:n.color,widgetDomain:window.location.toString().replace(/#.*$/,""),themeUrl:n.themeUrl,lang:n.lang};if(!n.offlineMode)for(e in o.readOnly=n.readOnly,s)s.hasOwnProperty(e)&&!o.hasOwnProperty(e)&&(o[e]=s[e]);for(e in o)o.hasOwnProperty(e)&&null!==o[e]&&i.push(e+"="+u(o[e]));if((t=this.getIframeDomain()+"?"+i.join("&")).length>2048)throw new Error("UWA.Embedded iframe url is more than 2048 characters please implement UWA.Embedded using offlineMode=true.");return t},getIframeDomain:function(){var e,t=this.options,i=t.exposition;return t.subDomain&&(e=r.getCheckSum(this.url),i=i.replace("://","://"+t.subDomainPattern.replace("{id}",e))),i+="/widget/frame"},initRemote:function(){var e,t=this,i=t.options;t.socket||(p.Servers[i.remoteName]||(p.Servers[i.remoteName]=new a.Server(i.remoteName)),(e=new a.Socket(t.id+"-master")).subscribeServer(i.remoteName,window,window.location.toString()),e.addListener("widgetMessage",function(e){var i=e.args,n=i.shift();t.disableRemote=n,t.dispatchEvent(n,i),t.disableRemote=!1}),t.socket=e,t._runRemoteQueue())},_runRemoteQueue:function(){var e,t;this.socket&&0!==this._remoteQueue.length&&(t=this._remoteQueue.shift(),!0===this.disableRemote||this.disableRemote===t[0]?this.log("sendRemote message ignored: "+t):(e={id:this.id,args:t},this.log("sendRemote message: "+t),this.socket.dispatchEvent("environmentMessage",e,[e.id+"-slave"])),this._runRemoteQueue())},sendRemote:function(){this._remoteQueue.push(r.toArray(arguments)),this._runRemoteQueue()},launch:function(e,t){void 0!==t&&(this.options.readOnly=t),void 0!==e&&(this.data=e),this.disableRemote=!1,this.sendRemote("launchWidget",this.data,this.options.readOnly)},setChromeColor:function(e){this.dispatchEvent("onColorize",[e]),this.sendRemote("onColorize",e)},setTitle:function(e){this.dispatchEvent("onUpdateTitle",[e]),this.sendRemote("onUpdateTitle",e)},setIcon:function(e,t){this.dispatchEvent("onUpdateIcon",[e,t]),this.sendRemote("onUpdateIcon",e,t)},setValue:function(e,t){this.dispatchEvent("onUpdateValue",[e,t]),this.sendRemote("onUpdateValue",e,t)},setValues:function(e){var t;for(t in e)e.hasOwnProperty(t)&&this.setValue(t,e[t])},resizeHeight:function(e,t){this.dispatchEvent("onResizeHeight",[e,t]),this.sendRemote("onResize")},resizeWidth:function(e,t){this.dispatchEvent("onResizeWidth",[e,t]),this.sendRemote("onResize")},onRegisterWidget:function(){var e=this.options;this.loadTime=(new Date).getTime(),this.disableRemote=!1,e.autoLaunch&&(e.offlineMode||e.useAsyncFrame)&&this.launch()},onUpdateTitle:function(e){this.title!==e&&(this.title=e,this.elements.title&&this.options.buildHeader&&null===this.options.title&&l(this.elements.title,{text:t.stripTags(e)}))},onUpdateIcon:function(e){if(this.icon!==e&&(this.icon=e,this.options.buildHeader)){var t=this.elements.icon,i=h("img",{src:e,onload:function(){t.src=e}});i.complete&&i.width>0&&(t.src=e)}},onUpdatePreferences:function(e){this.preferences=e},onUpdateValue:function(e,t){this.data[e]!==t&&(this.data[e]=t)},onResizeHeight:function(e,t){var i=this.options,n=i.maxHeight,s=n&&e>n;this.elements.iframe&&(t||"auto"===i.height)&&(this.elements.iframe.height=s?n:e)},onResizeWidth:function(e,t){var i=this.options;this.elements.iframe&&(t||"auto"===i.width)&&(this.elements.iframe.width=e)},onColorize:function(t){var i=this.options,n=this.elements;i.color=t,i.buildHeader&&(d(n.header,"transparent"!==t?{background:'url("'+i.uwa+e.paths.css+"themes/blueberry/img/moduleheader"+("white"!==t?"_"+t:"")+".png?v="+this.version+'") repeat-x scroll center top transparent'}:{background:null}),d(n.title,{color:"transparent"!==t?"white":"black"}))},onViewRequest:function(e){e||(e={}),e.error="No view implementation in Embedded mode",this.sendRemote("onViewError",e)},getCode:function(e){var t,i,n,s,o=this.url,r=JSON.stringify,a=this.options,d={},l=["/lib/c/UWA/js/UWA_Embedded.js"],h={uwa:a.uwa,exposition:a.exposition};for(n in a)a.hasOwnProperty(n)&&"container"!==n&&null!==a[n]&&this.defaultOptions[n]!==a[n]&&(c(a[n])||(d[n]=a[n]));if(e&&1===l.length)s=['<script type="text/javascript">',"var UWA = {hosts:"+r(h)+"}, UWA_ASYNC = UWA_ASYNC || [];",'    UWA_ASYNC.push({url: "'+o+'",options:'+r(d)+"});","(function () {",'    var a = document.getElementsByTagName("script"), b = a[a.length - 1] || document.body.lastChild,','        c = b.parentNode, d = document.createElement("script"), e = document.createElement("div");','    e.id = "UWA_ASYNC"; d.type = "text/javascript"; d.async = true;','    d.src = ("https:" == document.location.protocol ? "https://" : "http://") + UWA.hosts.uwa.split("://")[1] + "'+l[0]+"?v="+this.version+'";',"    c.insertBefore(d, b); c.insertBefore(e, b)","})();","<\/script>"];else{for((s=[]).push('<script type="text/javascript"> var UWA = {hosts:'+r(h)+"}; <\/script>"),t=0,i=l.length;t<i;t++)s.push('<script type="text/javascript" src="'+a.uwa+l[t]+"?v="+this.version+'"><\/script>');s.push('<script type="text/javascript">'),s.push('var MyWidget = new UWA.Embedded("'+o+'"'+(c(d)?"":","+r(d))+");"),s.push("<\/script>")}return s.join("\n")}});return p.Instances={},p.Servers={},function(){var t,i,n;if(window.UWA_ASYNC)for(n=window.UWA_ASYNC,e.Widgets=e.Widgets||[],t=0,i=n.length;t<i;t++)e.Widgets[t]=new p(n[t].url,n[t].options||{})}(),e.namespace("Embedded",p,e)});
define("UWA/Promise",["UWA/Core","UWA/Utils","UWA/Class","UWA/Internal/Deprecate"],function(e,t,r,n){"use strict";var i=Promise;function o(e){this._promise=e instanceof i?e:new i(e)}function a(e){return function(){return o.cast(this._promise[e].apply(this._promise,arguments))}}function c(e){return function(){return o.cast(i[e].apply(i,arguments))}}var s=o.prototype=Object.create(i.prototype);return s.constructor=o,s.catch=a("catch"),s.then=a("then"),s.fail=s.catch,s.finally=function(e){var t=this;function r(){return o.cast(e()).then(function(){return t})}return this.then(r,r)},s.fin=s.finally,s.done=function(e,r){return this.then(e,r).fail(function(e){var r=o.deferred();return t.setImmediate(function(){throw t.setImmediate(function(){r.reject(e)}),e instanceof Error?e:new Error(e)}),r.promise})},s.spread=function(e,t){return this.then(function(t){return e[Array.isArray(t)?"apply":"call"](null,t)},t)},o.race=c("race"),o.all=function(e){return"number"!=typeof e.length?o.reject(new TypeError("Not an iterable")):o.cast(i.all(t.toArray(e)))},o.reject=c("reject"),o.resolve=c("resolve"),o.cast=function(e){return e instanceof o?e:e instanceof i?new o(e):o.resolve(e)},o.deferred=function(){var e={},t=new o(function(t,r){return e.resolve=t,e.reject=r,e});return e.promise=t,e},o.allSettled=function(e){return o.all(t.toArray(e).map(function(e){return e instanceof i?e.then(function(e){return{state:"fullfilled",value:e}},function(e){return{state:"rejected",reason:e}}):{state:"fullfilled",value:e}}))},n.property(r,"Promise",{value:o,name:"UWA.Class.Promise",message:"Use UWA.Promise instead."}),e.namespace("Promise",o,e)});
define("UWA/Utils/Asset",["UWA/Promise","vendors/webcomponents/WeakMap"],function(e){"use strict";var t,n=new WeakMap;function r(e){return e.container.ownerDocument}function i(i,o){return function(a,c){return a=function(e){return t||(t=document.createElement("a")),t.href=e,t.href}(a),c=Object.assign({force:!1,timeout:6e4,container:document.head},c),function(e,t,i){if(t.force)return i();var o=r(t),a=n.get(o);return a||(a={},n.set(o,a)),a.hasOwnProperty(e)||(a[e]=i()),a[e]}(a,c,function(){var t,n,r=new e(function(e,r){t=o(a,c,e,r),n=setTimeout(function(){t(),r(new Error("Asset."+i+": Timeout while loading "+a))},c.timeout)});return r.fin(function(){clearTimeout(n)}),r})}}return{js:i("js",function(e,t,n,i){var o=r(t).createElement("script");return o.setAttribute("type","text/javascript"),o.addEventListener?(o.addEventListener("load",function(){n(o)}),o.addEventListener("error",function(){i(new Error("Asset.js: Error while loading "+e))})):o.attachEvent("onreadystatechange",function(){"loaded"!==o.readyState&&"complete"!==o.readyState||n(o)}),t.container.appendChild(o),o.src=e,function(){t.container.removeChild(o)}}),css:i("css",function(e,t,n,i){var o=r(t).createElement("link");return o.setAttribute("rel","stylesheet"),o.setAttribute("type","text/css"),o.addEventListener?(o.addEventListener("load",function(){n(o.sheet)}),o.addEventListener("error",function(){i(new Error("Asset.css: Error while loading "+e))})):o.attachEvent("onload",function(){n(o.styleSheet)}),t.container.appendChild(o),o.setAttribute("href",e),function(){t.container.removeChild(o)}})}});
define("UWA/Environment",["UWA/Core","UWA/String","UWA/Array","UWA/Class","UWA/Class/Timed","UWA/Class/Events","UWA/Class/Debug","UWA/Class/Options","UWA/Utils","UWA/Element","UWA/Event","UWA/Json","UWA/Data","UWA/Internal/StringMap","UWA/Widget","UWA/Controls/Form","UWA/Controls/WidgetPopupMenu","UWA/Embedded","UWA/Promise","UWA/Utils/Client","UWA/Utils/Asset"],function(e,t,n,i,s,o,r,a,c,l,d,u,h,f,p,v,m,g,w,E,y){"use strict";function b(t){var n=e.hosts.netvibes+"/subscribe.php",i={module:"UWA",moduleUrl:t.getUrl()};return t.getPreferences().forEach(function(e){i[e.name]=e.value}),n+"?"+c.toQueryString(i)}var W=Object.create(null),U=i.extend(s,o,r,a,{name:null,inited:!1,registered:!1,launched:!1,widget:null,html:null,features:{},views:{},menuClass:m,defaultOptions:{formOptions:{nativeInputs:!1},defaultView:{type:"windowed"},initialView:null},init:function(e){this.setOptions(e),this.html={},this.view={},this.dispatchInit()},dispatchInit:function(){var e=this;e.setPeriodical("init",function(){document.body&&!e.inited&&(e.clearPeriodical("init"),e.dispatchEvent("onInit"),e.inited=!0)},100,!0)},hasFeature:function(t,n){var i,s=e.owns(this.features,t)&&this.features[t];if(!s)return!1;if(n)for(i in n)if(e.owns(n,i)&&(!e.owns(s,i)||n[i]!==s[i]))return!1;return!0},getWidget:function(){var e=this.widget||new p;return this.widget||this.registerWidget(e),e},registerWidget:function(t){var n=this;n.widget=t,n.setPeriodical("register",function(){if(n.inited&&!n.registered){var i,s=n.html;for(i in n.clearPeriodical("register"),t.environment=n,s)s.hasOwnProperty(i)&&s[i]!==window&&(t.elements[i]=e.extendElement(s[i]));t.body=s.body,e.Widgets=e.Widgets||{},e.Widgets.instances=e.Widgets.instances||[],e.Widgets.instances.push(t),n.dispatchEvent("onRegisterWidget"),n.registerMenus(),n.registered=!0}},100,!0)},launchWidget:function(e,t){var n=this;n.setPeriodical("launch",function(){n.isDataReady()&&n.registered&&(n.clearPeriodical("launch"),n.getWidget().launch(e,t))},100,!0)},destroy:function(){var t,n,i=this.html,s=this.widget;for(t in s&&(e.Widgets.instances.splice(e.Widgets.instances.indexOf(s),1),s.destroy(),this.widget=null),this.clearDelayed(),this.clearPeriodical(),i)i.hasOwnProperty(t)&&l.destroy.call(i[t]);for(n in this.view)this.view.hasOwnProperty(n)&&this.view[n]&&this.view[n].destroy();this.removeEvent(),this.registered=!1,this.launched=!1},onInit:function(){},onRegisterWidget:function(){var e=this,t=e.html,n=e.widget;e.data=new f,t.menus&&l.addEvent.call(t.menus,"click",function(t){var n=d.getElement(t),i=e.widget.getMenu(n.getAttribute("data-name"));i&&(e.dispatchEvent("onMenuExecute",[i]),i.items&&(e.popupMenu||(e.popupMenu=new e.menuClass(e).inject(document.body)),e.popupMenu.setTarget(n).setItems(i.items).toggle()))}),t.editAction&&(l.show.call(t.editAction),l.addEvent.call(t.editAction,"click",function(t){d.stop(t),e.dispatchEvent("toggleEdit")})),t.refreshAction&&(l.show.call(t.refreshAction),l.addEvent.call(t.refreshAction,"click",function(t){d.stop(t),e.dispatchEvent("onRefresh")})),t.shareAction&&(t.shareAction.href=b(n),l.addEvent.call(t.shareAction,"click",function(t){d.stop(t),e.dispatchEvent("onOpenURL",b(n))})),t.wrapper&&l.handleExternalLinks.call(t.wrapper,function(t,n){e.dispatchEvent("onOpenURL",[t,n])}),(t.viewport||t.wrapper)&&l.addEvent.call(t.viewport||t.wrapper,"resize",function(){e.dispatchEvent("onResize")}),l.addEvent.call(document,"keydown",function(t){var n=t.which||t.keyCode;e.dispatchEvent("onKeyboardAction",[n,t])}),t.body&&[E.Engine.name,E.Engine.name+E.Engine.version,E.Platform.name,E.Features.touchEvents?"touch":"no-touch",n.readOnly&&"readonly",e.name&&"environment-"+e.name].forEach(function(e){e&&l.addClassName.call(t.body,e)}),e.dispatchEvent("onResize"),e.dispatchEvent("onViewRequest",[e.options.initialView])},registerMenus:function(){var t=this.getWidget();t.setMenu({name:"options",icon:"options"}),t.readOnly||t.setMenu({name:"options/preferences",icon:"cogwheel",label:e.i18n("Settings"),onExecute:"toggleEdit"}),t.setMenu({name:"options/refresh",icon:"refresh",label:e.i18n("Refresh"),onExecute:"onRefresh"})},onUpdateMenu:function(n){var i=this.html;i.menus&&(n||(n=this.widget.menus),i.menus.empty(),n.forEach(function(n){var s;!1!==(e.is(n.visible,"function")?n.visible():!1!==n.visible)&&(s=e.createElement("span",{class:"uwa-widget-menu-button","data-name":n.name}),n.help&&(s.set("title",n.help),s.set("uwa-tooltip",t.escapeHTML(n.help))),n.icon&&s.addClassName("uwa-icon "+n.icon),n.className&&s.addClassName(n.className),s.inject(i.menus),i.header&&i.header.set("data-menus-items",i.menus.childNodes.length))}))},onMenuExecute:function(t){e.is(t.onExecute,"string")&&this.widget.dispatchEvent(t.onExecute,[t])},isDataReady:function(){return!e.Storage||e.Storage.allInstancesReady()},getAllData:function(){return this.data.getAll()},getData:function(e){return this.log("getData:"+e),this.data.get(e)},setData:function(e,t){return this.log("setData:"+e+","+t),this.data.set(e,t)},deleteData:function(e){return this.log("deleteData:"+e),this.data.remove(e)},dispatchEvent:function(e,t,n,i){this.log("environment.event:"+e);var s=this.widget;!i&&s&&this.addEventOnce(e,s.dispatchEvent.bind(s,e,t,n,!0)),this._parent(e,t,n)},loadWidget:function(t,n){return n=e.extend({onFailure:function(e){throw e},onTimeout:function(e){throw e},onComplete:function(){}},n),t=c.buildUrl(window.location.toString(),t),n.embedded?this.loadEmbeddedWidget(t,n):this.loadInlinedWidget(t,n),this},loadInlinedWidget:function(){var t,i={};function s(e,t,s){i[e]&&(n.invoke(i[e],t,s),delete i[e])}return t=function(t,o){var r=o.expositionError||o.error||o.errors;if(!r||e.is(r,"array")&&0===r.length){(o=this.convertSourceToJson(o)).className||(o.checksum||(o.checksum=c.getCRC32(t)),o.className="w-"+o.checksum),o.style&&(c.setCss(o.className,o.style,"."+o.className,t),delete o.style),"string"==typeof o.script&&(o.script=new Function("widget",o.script)),o.styles=this.filterExternalResources("style",o.styles||[]),o.scripts=this.filterExternalResources("script",o.scripts||[]);for(var a=[];o.styles.length;)a.push(y.css(c.buildUrl(t,o.styles.shift())));for(;o.scripts.length;)a.push(y.js(c.buildUrl(t,o.scripts.shift())));w.all(a).done(function(){var s=i[t];i[t]=o,e.is(s,"array")&&n.invoke(s,"onComplete",o)},function(e){s(t,"onFailure",e)})}else s(t,"onFailure",r)},function(n,o){var r=i[n],a=o.fetcher||"XML",c=o.onComplete,l=this;return o.onComplete=function(e){var t=l.getWidget();t.uwaUrl=n,t.setTitle(e.title),t.setIcon(e.icon),t.setMetas(e.metas),t.setPreferences(e.preferences),t.setPlugins(e.plugins),t.setBody(e.body),l.html.wrapper.addClassName(e.className),e.script&&e.script(t),c(t,l)},e.is(r,"object")?o.onComplete(r):(e.is(r,"array")?r.push(o):i[n]=[o],o=e.merge({onComplete:t.bind(this,n),onTimeout:s.bind(this,n,"onTimeout"),onFailure:s.bind(this,n,"onFailure")},o),e.is(a,"function")?a.call(this,n,o):!e.is(a,"string")||a.length>4?o.onComplete(a):"JSON"===(a=a.toUpperCase())?this.fetchJsonWidget(n,o):this.fetchXmlWidget(n,o)),this}}(),loadEmbeddedWidget:function(t,n){var i,s,o=this,r=l.setStyle,a={cache:n.cache,container:o.html.body,displayHeader:!1,displayFooter:!1,displayEdit:!0,autoLaunch:!1};return e.is(n.embedded,"object")&&e.extend(a,n.embedded),i=new g(t,a),r.call(o.html.body,"padding",0),r.call(i.elements.body,"padding",0),o.addEvent("onRegisterWidget",function(){var e={},t={onUpdateValue:!0,onRefresh:!0,onUpdateTitle:!0,onUpdateIcon:!0,onUpdateCounter:!0,onSearch:!0,onResetSearch:!0,onShowEdit:!0,onKeyboardAction:!0,onViewError:!0,onViewChange:!0,onEdit:!0,endEdit:!0,onLoad:function(){i.launch(o.getAllData(),o.getWidget().readOnly)}};Object.keys(t).forEach(function(n){var s=t[n];!0===s&&(s=i.sendRemote.bind(i,n)),e[n]=s}),o.addEvents(e)}),s=o.getWidget(),i.addEvent("onRegisterWidget",function(){var t={},r={onRefresh:!0,onUpdateTitle:!0,onUpdateIcon:!0,onUpdateCounter:!0,onSearch:!0,onResetSearch:!0,onHideEdit:!0,onShowEdit:!0,onOpenURL:!0,onViewRequest:!0,onInitConfig:function(e){e.preferences&&s.setPreferences(e.preferences),e.plugins&&s.setPlugins(e.plugins),e.metas&&s.setMetas(e.metas)},onUpdatePreferences:function(e){s.setPreferences(e)},onUpdateValue:function(e,t){s.setValue(e,t)}};a.displayEdit||e.merge(r,{onEdit:!0,endEdit:!0}),Object.keys(r).forEach(function(e){var n=r[e];!0===n&&(n=function(){s.dispatchEvent(e,arguments)}),t[e]=n}),i.addEvents(t),n.onComplete(s,o)}),o.embedded=i,o},convertSourceToJson:function(){var t=["name","defaultValue","type","label","step","min","max"],n=["label","value"],i=/(java|ecma)script$/i;function s(e,t,n){var i,s,o,r=[].slice.call(e.childNodes);for(i=0,s=r.length;i<s;i++)o=r[i],n&&1!==o.nodeType||t(o,o.nodeValue)}function o(e,t){var n,i,s,o=e.attributes||[];for(n=0,i=o.length;n<i;n++)t((s=o[n]).name,s.value)}var r={"widget:preferences":function(e,i){s(i,function(i){var r,a={};o(i,function(e,n){-1!==t.indexOf(e)&&(a[e]=n)}),a.name&&("list"!==a.type&&"checklist"!==a.type||(r=[],s(i,function(e){var t={};o(e,function(e,i){-1!==n.indexOf(e)&&(t[e]=i)}),t.label&&r.push(t)},!0),a.options=r),e.preferences.push(a))},!0)},"widget:plugins":function(e,t){s(t,function(n){var i={name:t.getAttribute("name"),options:{}};o(n,function(e,t){i[e]=t}),s(n,function(e){var t=e.getAttribute("name"),n=e.getAttribute("value");"widget:options"===e.tagName?(i.options[t]={},s(e,function(e){var n=e.getAttribute("name"),s=e.getAttribute("value");n&&(i.options[t][n]=s)},!0)):t&&(i.options[t]=n)},!0),i.name&&e.plugins.push(i)})},link:function(e,t,n){if(n.href){var i=n.rel;"icon"===i?e.icon=n.href:"stylesheet"!==i||n.href.contains("UWA/assets")||n.href.contains("standalone.css")||n.href.contains("uwa/style.css")||e.styles.push(n.href)}},meta:function(e,t,n){var i=n.content;i="false"!==i&&("true"===i||i),e.metas[n.name]=i},script:function(e,t,n){if(n.src||(n.language||n.type)&&!i.test(n.type)&&!n.language){if(!n.src||n.src.contains("Standalone")||n.src.contains("load.js.php"))return t;e.scripts.push(n.src)}else{var o="";s(t,function(e,t){o+=t}),/UWA(\s+)?=/.test(o)||(e.script+=o)}},title:function(e,t){s(t,function(t,n){e.title+=n})},style:function(e,t){s(t,function(t,n){e.style+=n})},fallback:function(e,t,n,i){var r;return"body"===i?((r=document.createElement("div")).className=t.className,e.body=r):r=document.createElement(i),o(t,function(e,t){r.setAttribute(e,t)}),s(t,function(t,n){switch(t.nodeType){case 1:var i=a(t,e);i&&r.appendChild(i);break;case 4:case 3:r.appendChild(document.createTextNode(n))}}),r}};function a(e,t){9===e.nodeType&&(e=e.childNodes[0]);var n=e.nodeName.toLowerCase(),i={};return o(e,function(e,t){i[e]=t}),r[r.hasOwnProperty(n)?n:"fallback"](t,e,i,n)}return function(t){if(e.is(t,"string"))try{t=c.loadXml(t)}catch(n){e.log("Invalid UWA XHTML source detected, fallback on HTML parsor."),t=c.loadHtml(t)}var n;return e.is(t,"object")?n=t:a(t,n={title:"",icon:"",preferences:[],plugins:[],metas:{},body:[],script:"",scripts:[],style:"",styles:[]}),n}}(),fetchJsonWidget:function(t,n){t in W||(W[t]=new w(function(i,s){var o,r={mode:"full",uwaUrl:t};e.debug&&(r.flush=1,r.mode="full_debug"),o=(n.server||e.hosts.exposition)+"/widget/json",u.request(o,{data:r,onComplete:i,onFailure:s,useJsonpRequest:!0,callback:t})})),W[t].then(n.onComplete,n.onError)},fetchXmlWidget:function(e,t){h.request(e,{cache:t.cache,type:"text",onFailure:t.onFailure,onTimeout:t.onTimeout,onComplete:t.onComplete})},filterExternalResources:function(e,t){return t},onRefresh:function(){var e=this.getWidget();e.data={},e.hasEvent("onRefresh")||e.dispatchEvent("onLoad",void 0,void 0,!0)},onUpdateIcon:function(t){var n=this.html;function i(){n.iconLoader.destroy(),delete n.iconLoader}n.icon&&(n.iconLoader&&i(),n.iconLoader=e.createElement("img",{styles:{display:"none"},events:{load:function(){n.icon.getElement("img").setAttribute("src",t),i()},error:function(){i()}}}).inject(this.html.wrapper),n.iconLoader.setAttribute("src",t))},onUpdateTitle:function(e){var t=this.html.title;t&&t.setHTML(e)},onUpdateCounter:function(e){var t=this.html.counter;t&&t.setText(e?"("+(!0===e?"●":e)+")":"")},onEdit:function(){var t=this,n=t.html,i=t.getWidget(),s=i.metas,o=i.getPreferences();if(n.edit){if(n.edit.empty(),i.hasPreferences()){if(n.preferences){var r=n.preferences.getFormValues();o.forEach(function(t){e.is(r[t.name])&&(t.value=r[t.name])})}o.push({type:"submit",name:"endEdit",value:e.i18n("Done")}),n.preferences&&n.preferences.destroy(),n.preferences=new v({nativeInputs:this.options.formOptions.nativeInputs,darkBackground:this.options.formOptions.darkBackground,fields:o,events:{onChange:function(e,n,s){i.setValue(n,s),t.embedded?t.embedded.sendRemote("dispatchEvent",e,n,s):t.dispatchEvent(e,[n,s])},onSubmit:function(e,n){var s=!1;t.addEventOnce("onUpdateValue",function(){s=!0}),Object.keys(n).forEach(function(e){i.setValue(e,n[e])}),t.dispatchEvent("endEdit"),s&&t.dispatchEvent("onRefresh")}}}).inject(n.edit)}s.author&&n.edit.addContent({tag:"div",class:"moduleInfos",html:[{tag:"p",html:[e.i18n("Widget by")+" ",{tag:"strong",html:s.website?{tag:"a",href:s.website,text:s.author}:{tag:"span",text:s.author}}]}]})}t.dispatchEvent("onShowEdit")},onShowEdit:function(){var e=this.html;e.wrapper&&e.wrapper.addClassName("onEdit")},endEdit:function(){this.dispatchEvent("onHideEdit")},onHideEdit:function(){var e=this.html;e.wrapper&&e.wrapper.removeClassName("onEdit")},onCloseEdit:function(){this.html.preferences.destroy(),this.html.preferences=null},onOpenURL:function(n){if(n=c.parseUrl(n),!window.open(n.source,"_blank"))return window.alert(t.format(e.i18n('Unable to open "{0}", Please turn off your popup blocker and try again.'),t.truncate(n.source,50))),!1},onViewRequest:function(){function t(e,t,n){n&&(t.error=n),e.dispatchEvent(n?"onViewError":"onViewChange",[t])}function n(e,t,n){e[t]&&e[t].destroy(),e[t]=n}return function(i){var s;i||(i=this.options.defaultView),i=e.clone(i),this.view.current&&this.view.current.event&&(i.previous=e.clone(this.view.current.event),delete i.previous.previous),this.view.current&&this.view.current.matchEvent(i)?t(this,i,"This view is already active."):(s=function e(i,s){var o=i.views[s.type],r=o&&new o(i,s);return r&&r.addEvents({onEnter:function(){i.view.next===this&&(n(i.view,"current",this),this.isSingle()&&(U._currentSingleView=this),i.view.next=null,t(i,this.event))},onLeave:function(){i.view.current===this&&(U._currentSingleView===this&&(U._currentSingleView=null),i.view.next||(i.view.next=e(i,i.options.defaultView)),i.view.next.enter())},onError:function(e){i.view.next===this&&(n(i.view,"next"),i.view.current.enter()),t(i,this.event,e)}})}(this,i))?s.isSingle()&&U._currentSingleView&&U._currentSingleView!==this.view.current?(t(this,i,"An environment is already in single view."),s.destroy()):(n(this.view,"next",s),this.view.current?this.view.current.leave():this.view.next.enter()):t(this,i,'No implementation available for the view "'+i.type+'".')}}(),onViewChange:function(e){this.getWidget()._view=e},onViewError:function(e){this.log("View error: "+u.encode(e))}});return U.AbstractView=i.extend(o,{event:null,environment:null,init:function(e,t){this.environment=e,this.event=t},destroy:function(){this.removeEvents(),U._currentSingleView===this&&(U._currentSingleView=null)},enter:function(){this.dispatchEvent("onEnter")},leave:function(){this.dispatchEvent("onLeave")},isSingle:function(){return!1},matchEvent:function(e){return this.event.type===e.type},onEnter:function(){var e=this.environment.html;e.wrapper&&e.body&&n.invoke([e.wrapper,e.body],"addClassName",this.event.type+"-view")},onLeave:function(){var e=this.environment.html;e.wrapper&&e.body&&n.invoke([e.wrapper,e.body],"removeClassName",this.event.type+"-view")}}),U.prototype.views.windowed=U.AbstractView.extend({}),E.Features.fullscreen&&(U.prototype.views.fullscreen=U.AbstractView.extend({enter:function(){var e,t=this,n=t.getTarget();e={fullscreenchange:function(){document.fullscreenElement===n?t.dispatchEvent("onEnter"):(t.dispatchEvent("onLeave"),l.removeEvents.call(document,e))},fullscreenerror:function(){t.dispatchEvent("onError",["Error while trying to set the fullscreen"]),l.removeEvents.call(document,e)}},l.addEvents.call(document,e),n.requestFullscreen()},leave:function(){document.fullscreenElement===this.getTarget()?document.exitFullscreen():this.dispatchEvent("onLeave")},isSingle:function(){return!0},getTarget:function(){var e=this.environment.html;return e.content||e.body}})),e.namespace("Environment",U,e)});
define("UWA/Class/Promise",["UWA/Core","UWA/Promise","UWA/Internal/Deprecate"],function(e,s,r){"use strict";return r.warn("Module UWA/Class/Promise","Use UWA/Promise instead"),e.namespace("Class/Promise",s,e,"replace")});
define("UWA/Drivers/Alone",["UWA/Internal/Deprecate","UWA/Core","UWA/Event","UWA/Function","UWA/String","UWA/Array","UWA/Date","UWA/Object","UWA/Utils","UWA/Class","UWA/Dispatcher","UWA/Utils/Client","UWA/Ajax","UWA/Json","UWA/Storage","UWA/Data","UWA/Element","UWA/Fx","UWA/Plugins/Abstract","UWA/Controls/Pager","UWA/Controls/Img","UWA/Controls/Form","UWA/Widget","UWA/Environment","UWA/Promise","UWA/Class/Promise"],function(A,U){"use strict";return A.warn("UWA/Drivers/*","Don't use UWA drivers."),U});
define("UWA/Controls/Calendar",["UWA/Core","UWA/Date","UWA/Event","UWA/Controls/Abstract","UWA/String"],function(e,t,i,n,s){"use strict";var a,r=e.i18n;function l(e,t){var i=!e;return i===!t&&(i||e.getFullYear()===t.getFullYear()&&e.getMonth()===t.getMonth()&&e.getDate()===t.getDate())}function h(e,t,i){var n=e.getDate();if(void 0===i&&(i=1),"year"===t?(i*=12,t="month"):"week"===t&&(i*=7,t="day"),"month"===t)e.setDate(1),e.setMonth(e.getMonth()+i+1),e.setDate(0),n<e.getDate()&&e.setDate(n);else{if("day"!==t)throw new Error('Unknown unit "'+t+'"');e.setDate(n+i)}}return a=n.extend({name:"uwa-calendar",defaultOptions:{view:"month",weekFirstDay:"monday",limit:{}},weekOffset:{monday:1,sunday:0,saturday:6},init:function(e){this._parent(e),this.buildSkeleton(),this.bound={refreshLimit:this.refreshLimit.bind(this)},this.setLimit(this.options.limit),this.setDate(this.options.date),this.displayView(this.options.view)},getWeekOffset:function(){return this.weekOffset[this.options.weekFirstDay]||0},getMonthFirstDay:function(){var e=this.displayDate;return(new Date(e.getFullYear(),e.getMonth(),1).getDay()-this.getWeekOffset()+7)%7},getWeekFirstDay:function(){var e=this.displayDate;return e.getDate()-(7+e.getDay()-this.getWeekOffset())%7},iterateWeek:function(e,t){var i,n=this.displayDate,s=new Date(n.getFullYear(),n.getMonth(),this.getWeekFirstDay()),a=s.getDate();for(i=0;i<7;i+=1){var r=new Date(s);r.setDate(a+i),e.call(t,i,r)}return this},displayView:function(e){if(["month","week"].indexOf(e)<0)throw new Error("Unknown view "+e+"options");return e!==this.currentView&&(this.container.setContent(this["build"+s.ucfirst(e)+"View"]()),this.currentView=e,this.dispatchEvent("onRefresh")),this},setDate:function(e,t){t||(e||((e=new Date).setHours(0),e.setMinutes(0),e.setSeconds(0),e.setMilliseconds(0)),t=e);var i=!l(e,this.selectDate);return!i&&l(t,this.displayDate)||(this.selectDate=e,this.displayDate=t,this.dispatchEvent("onRefresh"),i&&this.dispatchEvent("onDateChange",[e])),this},getDate:function(){return this.selectDate||null},setLimit:function(e){e||(e={});var t=this.options.limit;return this.options.limit=e,[t.max,t.min,e.max,e.min].forEach(function(e,t){e instanceof a&&e[t<2?"removeEvent":"addEvent"]("onDateChange",this.bound.refreshLimit)},this),this.refreshLimit(),this},getLimit:function(){var e,t,i,n=this.options.limit||{},s={};for(e=0;e<2;e+=1)i=n[t=e?"max":"min"],s[t]=i&&new Date((i.getTime||i.getDate||i).call(i)).getTime()||(e?1/0:-1/0);return s.min-=864e5,s},refreshLimit:function(){var e=this.getLimit();if(e.end<e.start)throw new Error("Bad limit specified");return this.selectDate&&(this.preventRefresh(),this.setDate(new Date(Math.max(Math.min(e.max,this.selectDate),e.min))),this.allowRefresh()),this.dispatchEvent("onRefresh")},preventRefresh:function(){return this.doNotRefresh=this.doNotRefresh+1||1,this},allowRefresh:function(){return this.doNotRefresh=this.doNotRefresh-1||0,this},buildSkeleton:function(){this.container=e.createElement("div",{class:this.getClassNames(),events:{click:this.onClick.bind(this),mousedown:i.preventDefault}})},buildMonthView:function(){var i,n,s,a=e.createElement("div",{class:"monthView"}),r=e.createElement("div",{class:"top"}).inject(a),l=e.createElement("table").inject(a),h=e.createElement("tbody").inject(l),o=e.createElement("tr").inject(h);for(this.iterateWeek(function(i,n){e.createElement("th",{text:t.strftime(n,"%a")[0]}).inject(o)}),n=0;n<42;n+=1)n%7==0&&(i=e.createElement("tr").inject(h)),s=e.createElement("td").inject(i),e.createElement("div",{class:"day"}).inject(s);return e.createElement("span",{class:"previous uwa-icon","data-icon":"l"}).inject(r),e.createElement("span",{class:"title"}).inject(r),e.createElement("span",{class:"next uwa-icon","data-icon":"m"}).inject(r),this.elements.monthView=a,a},buildWeekView:function(){var i,n,s=e.createElement("div",{class:"weekView"}),a=e.createElement("div",{class:"top"}).inject(s),r=e.createElement("table").inject(s),l=e.createElement("tbody").inject(r),h=e.createElement("tr").inject(l);for(this.iterateWeek(function(i,n){e.createElement("th",{text:t.strftime(n,"%a")[0]}).inject(h)}),n=0;n<7;n+=1)n%7==0&&(i=e.createElement("tr").inject(l)),e.createElement("td",{html:{tag:"div",class:"day"}}).inject(i);return e.createElement("span",{class:"previous",text:"←"}).inject(a),e.createElement("span",{class:"title"}).inject(a),e.createElement("span",{class:"next",text:"→"}).inject(a),this.elements.weekView=s,s},refreshMonthView:function(){var e,i,n=this.displayDate,s=new Date(n.getFullYear(),n.getMonth(),-this.getMonthFirstDay()),a=this.elements.monthView,l=a.getElements(".day");for(e=0,i=l.length;e<i;e+=1)s.setDate(s.getDate()+1),l[e]=this.buildDay(l[e],s);a.getElement("tbody").getElements("tr")[6][s.getDate()>6?"hide":"show"](),a.getElement(".title").setText(t.strftime(n,r("%B %Y")))},refreshWeekView:function(){var e,i,n,s=this.displayDate,a=new Date(s.getFullYear(),s.getMonth(),this.getWeekFirstDay()),l=t.strftime(a,r("%e %B")),h=this.elements.weekView,o=h.getElements(".day");for(e=0,i=o.length;e<i;e+=1)o[e]=this.buildDay(o[e],a),a.setDate(a.getDate()+1);a.setDate(a.getDate()-1),n=t.strftime(a,r("%e %B %Y")),h.getElement(".title").setText(l+" - "+n)},buildDay:function(e,t){var i=new Date,n=this.displayDate,s=this.getLimit();return e.getClosest("td").toggleClassName("currentDay",l(t,n)).toggleClassName("selectDate",l(t,this.selectDate)).toggleClassName("today",l(t,i)).toggleClassName("currentMonth",t.getMonth()===n.getMonth()).toggleClassName("disabled",t<s.min||t>s.max),e.setText(t.getDate()),e},onRefresh:function(){var e=this.currentView;e&&!this.doNotRefresh&&this["refresh"+s.ucfirst(e)+"View"]()},onClick:function(e){var t,n=this.container,s=i.getElement(e),a=s.hasClassName("next")?1:s.hasClassName("previous")?-1:0,r=new Date(this.displayDate);s.getClosest(".disabled")||(s.hasClassName("day")?(h(r,"day",(t=n.getElements(".day")).indexOf(s)-t.indexOf(n.getElement(".currentDay .day"))),this.setDate(r),this.dispatchEvent("onDateSelect",[r])):a&&(h(r,this.currentView,a),this.setDate(this.selectDate,r)))}}),e.namespace("Controls/Calendar",a,e)});
define("UWA/Controls/Picker",["UWA/Core","UWA/Utils","UWA/Event","UWA/Class/Timed","UWA/Controls/Input","UWA/Controls/DropDown","UWA/Element"],function(t,n,e,o,i,s,a){"use strict";var l=i.extend(o,{name:"uwa-picker",options:{navigation:null,button:null,valueInput:"text",dropdownOptions:{global:!0},dropdownContainer:null},buildSkeleton:function(){var n=this.options,e=this.elements;this._parent(),n.valueInput&&n.button?e.content.addClassName(this.getClassNames("-split")):n.button?e.container.addClassName("button-only"):n.valueInput&&e.container.addClassName("value-only"),n.valueInput&&(e.content.setContent(e.value=t.createElement("div",{class:this.getClassNames("-value")})),"text"===n.valueInput&&e.value.addClassName(this.getClassNames("-text"))),n.button&&e.content.addContent(e.button=t.createElement("div",{class:this.getClassNames("-button"),html:n.button}))},buildContent:function(){},buildNavigation:function(e){return n.splat(e).map(function(n){return t.is(n,"element")?n:this.buildNavigationItem(n)},this)},buildNavigationItem:function(n){var e=this;return t.createElement("div",{text:n.label,class:this.getClassNames("-navigationlink"),events:{click:function(t){e.dispatchEvent("onNavigationClick",[t,n])}}})},syncInput:function(){var t=this.elements.value;t!==this.elements.input&&t.setText(this.getValue())},isOpen:function(){return Boolean(this.elements.dropdown&&this.elements.dropdown.isOpen())},focus:function(t){var n=this,e=n._parent;setTimeout(function(){var o=document.activeElement,i=n.elements.dropdown;o&&i&&a.isInjected.call(o,i.getInnerElement())?a.addEvent.call(o,"blur",function t(){a.removeEvent.call(o,"blur",t),n.focus(!1)}):(e.call(n,t),!1===t&&n.toggle(t))},0)},open:function(){return this.toggle(!0)},close:function(){return this.toggle(!1)},toggle:function(n){var o=this.elements,i=this.options;if((!0===n||void 0===n)&&!o.dropdown){var a=t.extend({target:o.button||o.content,autoPosition:["below-end","right-start","above-end","left-start"]},i.dropdownOptions);a._root=!1,a.className=this.getClassNames("-dropdown")+" "+(a.className||""),o.dropdown=new s.Pointy(a).addEvents({onShow:this.dispatchEvent.bind(this,"onOpen"),onHide:this.dispatchEvent.bind(this,"onClose")}),i.navigation&&(o.navigation=t.createElement("div",{class:this.getClassNames("-navigation"),html:this.buildNavigation(this.options.navigation)})),o.dropdown.getInnerElement().addEvent("mousedown",e.stopPropagation).addEvent("click",e.stopPropagation).addContent({tag:"div",class:this.getClassNames("-selector"),html:this.buildContent()},o.navigation),o.dropdown.inject(i.dropdownContainer||o.container)}o.dropdown&&o.dropdown.toggle(n)},onClick:function(){this.setDelayed("debounced-toggle",this.toggle,1)},onOpen:function(){this.elements.container.addClassName("open")},onClose:function(){this.elements.container&&this.elements.container.removeClassName("open")},onNavigationClick:function(t,n){this.setValue(n.value)}});return t.namespace("Controls/Picker",l,t)});
define("UWA/Controls/DatePicker",["UWA/Core","UWA/Date","UWA/Event","UWA/Controls/Calendar","UWA/Controls/Abstract","UWA/Controls/Picker"],function(e,t,n,a,i,s){"use strict";var o;return o=s.extend({name:"uwa-datepicker",options:{format:"%x",calendarOptions:{},button:{tag:"div",class:"uwa-icon uwa-icon-only calendar"},time:!1,utc:!1},setOptions:function(e){return e||(e={}),e.date&&(e.value=e.date/1e3),this._parent(e)},syncInput:function(){var e=this.elements,n=this.getDate();e.value&&e.value.setText(n?t.strftime(n,this.options.format):""),e.calendar&&e.calendar.setDate(n),e.time&&n&&(e.time.getElement(".value").setText(t.strftime(n,"%x")),e.time.getElements("input").forEach(function(e){e.value=n["get"+e.getAttribute("data-action")]()||""}))},onChange:function(){this.dispatchEvent("onDateSelect",[this.getDate()])},onOpen:function(){this._parent();var e=this.elements;e.calendar.refreshLimit(),e.time&&(e.time.hide(),e.calendar.show())},buildContent:function(){var t,i=this;return t=function(e){var t=this,a=n.whichKey(e);1===a.length&&isNaN(a)&&n.preventDefault(e),setTimeout(function(){var e,n,a=i.getDate()||new Date;a["set"+t.getAttribute("data-action")](t.value),i.setDate(a),t.value.length>=2&&(n=((e=i.elements.time.getElements("input")).indexOf(t)+1)%e.length,e[n].select())},1)},i.options.time&&(i.elements.time=e.createElement("div",{class:i.getClassNames("-time"),html:[{tag:"div",class:"value"},{tag:"input",type:"text",class:i.getClassNames("-text"),"data-action":"Hours",events:{keydown:t}},":",{tag:"input",type:"text",class:i.getClassNames("-text"),"data-action":"Minutes",events:{keydown:t}}]}).hide()),i.elements.content=e.createElement("div",{html:[i.elements.calendar=new a(e.extend({_root:!1},i.options.calendarOptions)).setDate(this.getDate()).addEvent("onDateSelect",function(e){var t=i.getDate();t?(t.setDate(e.getDate()),t.setMonth(e.getMonth()),t.setFullYear(e.getFullYear())):t=e,i.setDate(t),i.options.time?(i.elements.calendar.hide(),i.elements.time.show().getElement("input").select(),i.elements.dropdown.updatePosition()):(i.toggle(!1),i.dispatchEvent("onChange",[i.getValue()]))}),i.elements.time]}),i.elements.content},buildNavigationItem:function(e){return e.date&&(e.value=e.date/1e3),this._parent(e)},setDate:function(e){return e&&this.options.utc&&(e=e.getTime()-6e4*e.getTimezoneOffset()),this.setValue(e/1e3||"")},getDate:function(){var e=this.getValue();if(e)return this.options.utc&&(e=Number(e)+60*(new Date).getTimezoneOffset()),new Date(1e3*e)},setLimit:function(e){return this.elements.calendar?this.elements.calendar.setLimit(e):this.setOptions({calendarOptions:{limit:e}}),this}}),e.namespace("Controls/DatePicker",o,e)});
/*global define */ 
 define("DS/W3DPassport/dsp/component/HiddenInput", [
     "UWA/Controls/Input"
 ], function (Input) {
    "use strict";
    
    Input.Hidden = Input.extend({
        name: "uwa-hidden",
        _hiddenInput: false, /* false : hidden but not emulated */

        buildInput: function () {
            return UWA.createElement('input', { type: 'hidden'});
        },

        buildSkeleton: function () {
            this._parent();
            this.elements.input.addClassName(this.getClassNames('-hidden'));
        }
    }); 
 });


/*global define */
 define("DS/W3DPassport/dsp/component/PasswordInput", [
     "UWA/Controls/Input"
 ], function (Input) {
    "use strict";

    Input.Password = Input.extend({
        name: "uwa-password",

        _hiddenInput: false,
        
        init: function(options) {
            this._parent(options);
            this.buildSkeleton();
        },

        buildInput: function () {
            return UWA.createElement('input', { type: 'password'});
        },

        buildSkeleton: function () {
            this._parent();
            this.elements.input.addClassName(this.getClassNames('-password'));
        }
    });
 });


/*global define */
 define("DS/W3DPassport/dsp/component/SubmitInput", [
     "UWA/Controls/Input"
 ], function (Input) {
    "use strict";

    Input.Submit = Input.extend({
        name: "uwa-submit",

        _hiddenInput: false,

        buildInput: function () {
            return UWA.createElement('input', { type: 'submit'});
        },

        buildSkeleton: function () {
            this._parent();
            this.elements.input.addClassName(this.getClassNames('-submit'));
        }
    });
 });


/*global define */
/*jslint nomen: true */
define("DS/W3DPassport/dsp/component/InputForm", [
    "UWA/Core",
    "UWA/Controls/Abstract",
    "UWA/Controls/Input",
    "UWA/Controls/Form"
], function (UWA, Abstract, Input, Form) {
    "use strict";

    var Form = Abstract.extend({
        defaultOptions: {
            className: 'uwa-input-form',
            fields: [],
            commands: [],
            labelPreffix: ':'
        },

        init: function (options) {
            this._parent(options);
            this.elements.inputs = {};
            this.buildSkeleton();
        },

        buildSkeleton: function () {
            var options = this.options,
                form,
                fieldset,
                commands;

            form = UWA.createElement('form', {
                'class': options.className,
                events: {
                    submit: function (event) {
                        UWA.Event.stop(event);
                        this.dispatchEvent('onSubmit', [event, this.getFormValues()]);
                    }.bind(this)
                }
            });
            // Wrap all fields in a fieldset tag.
            fieldset = this.createFieldSet(options);
            fieldset.inject(form);
            commands = this.createCommands(options.commands);
            commands.inject(form);
            this.elements.container = form;
        },

        /**
         * Create a fieldset tag and its content according to the given
         * fieldsetDef object.
         *
         * @param {Object} fieldsetDef
         * @param {String} fieldsetDef.type         must be "fieldset" (undefined for the fieldset wrapper create by the form).
         * @param {String} fieldsetDef.className    optional parameter to add a custom css class.
         * @param {Array}  fieldsetDef.fields       An Array of fieldDef.
         *
         * @returns {UWA.Element} A fieldset UWA.Element.
         */
        createFieldSet: function (fieldsetDef) {
            var fieldset,
                legend,
                fieldDefs = fieldsetDef.fields || [],
                fieldDef,
                field,
                len,
                i,
                myAttributes = fieldsetDef.attributes;

            fieldset = new UWA.createElement('fieldset', myAttributes);
            if (undefined !== fieldsetDef.legend) {
            	var legend = fieldsetDef.legend,
            		legendValue,
            		legendAttributes;
            	if(typeof legend === 'string') {
            		legendValue = legend;
            		legendAttributes = {};
            	} else {
            		legendValue = legend.value;
            		legendAttributes = legend.attributes;
            	}
                legend = new UWA.createElement('legend', {
                    "class": "section-title",
                    text: legendValue,
                    attributes: legendAttributes
                });
                legend.inject(fieldset);
            }
            len = fieldDefs.length;
            for (i = 0; i < len; i += 1) {
                fieldDef = fieldDefs[i];
                if ("fieldset" === fieldDef.type) {
                    field = this.createFieldSet(fieldDef);
                } else {
                    field = this.createField(fieldDef);
                }
                field.inject(fieldset);
            }
            return fieldset;
        },

        /**
        * Create a field to be added to the form. The field is a component that contains
        * a wrapper a label and a input.
        *
        * @param {Object} fieldDef
        * @param {String} fieldDef.type     Should be one of the property of the
        *                                   InputForm.inputFactory Object.
        * @param {String} fieldDef.label    The text displayed as a label for the input (translated by UWA.i18n).
        * @param {String} fieldDef.name     The name attribute of the input.
        * @param {String} fieldDef.value    The value attribute of the input.
        * @returns {UWA.Element} An element that represent an entry in the form.
        */
        createField: function (fieldDef) {
            var inputFactory = this.inputFactory,
                field,
                label,
                input;

            if (fieldDef.label) {
                label = [{
                    tag: "span",
                    "class": "label",
                    text: UWA.i18n(fieldDef.label)
                }];
            }
            field = UWA.createElement("div", {
                "class": "field " + (fieldDef.className || ""),
                html: [{
                    tag: "label",
                    html: label
                }]
            });
            if (undefined === this.inputFactory[fieldDef.type]) {
                fieldDef.type = "text";
            }
            input = this.inputFactory[fieldDef.type](fieldDef);
            input.inject(field.getElement("label"));
            this.elements.inputs[fieldDef.attributes.name] = input;
            return field;
        },

        /**
         *
         * @param {Array} commandsDefs An array of configuration object for command UWA.Input inputs.
         * @returns {UWA.Element} An element that represents the commands of the form.
         */
        createCommands: function (commandsDefs) {
            var commands,
                command,
                commandDef,
                len,
                i;

            commands = UWA.createElement("div", {
                "class": "commands"
            });
            len = commandsDefs.length;
            for (i = 0; i < len; i += 1) {
                commandDef = commandsDefs[i];
                if (undefined === this.inputFactory[commandDef.type]) {
                    commandDef.type = "button";
                }
                command = this.inputFactory[commandDef.type](commandDef);
                command.inject(commands);
            }

            return commands;
        },

        inputFactory: {
            text: function (options) { options.className="form-control form-control-root "; return new Input.Text(options); },
            email: function (options) { return new Input.Text(options); },
            button: function (options) { options.className=""; return new Input.Button(options); },
            list: function (options) { return new Input.Select(options); },
            select: function (options) { return new Input.Select(options); },
            checkbox: function (options) { options.className="aligned-checkbox"; return new Input.Checkbox(options); },
            number: function (options) { options.attributes.type="number"; return new Input.Text(options); }
        },

        getFields: Form.prototype.getFields,
        getFormValues: Form.prototype.getFormValues
    });

    return UWA.namespace('dsp/component/InputForm', Form, UWA);
});

/*global define */
/*jslint nomen: true */
define("DS/W3DPassport/dsp/component/Panel", [
    "UWA/Core",
    "UWA/Controls/Abstract"
], function (UWA, Abstract) {
    "use strict";

    var Panel = Abstract.extend({

        container: undefined,

        defaultOptions: {
            className: "",
            title: "",
            "data-dsp-i18n": ""
        },

        init: function (options) {
            this._parent(options);
            this.buildSkeleton();
            this.elements = [];
        },

        /**
         *
         * @returns {undefined}
         */
        buildSkeleton: function () {
            var options = this.options;

            this.container = UWA.createElement("div", {
                "class": "uwa-panel"
            });
            this.container.addClassName(options.className);
            if (options.title) {
                this.addTitle(options.title);
            }
        },

        /**
         *
         * @param {String} title
         * @returns {undefined}
         */
        addTitle: function (title) {
            var titleElt,
                titleString,
                isString = typeof title === 'string';

            if('link' === title.type) {
            	var elt = {
					tag: "a",
					href: title.href,
					text: title.title
				}
				if(title["data-dsp-i18n"]) {
					elt["data-dsp-i18n"] = title["data-dsp-i18n"];
				}
                titleElt = UWA.createElement("h1",{
                    "class": "panel-title panel-title-complex",
                    html: [elt]});
                titleElt.inject(this.container, "top");
            } else {
                if(isString) {
                    titleString = title;
                } else {
                    titleString = title["data-dsp-i18n"];
                }
                var structure = {
                    "class": "panel-title",
                    text: UWA.i18n(titleString)
                };
                if(!isString) {
                    structure.attributes = title;
                }
                //titleElt = UWA.createElement("h1",structure );
                titleElt = UWA.createElement("h3",structure );
                titleElt.inject(this.container, "top");
            }
        },

        addContentElement:  function (element) {
            if ("function" === typeof element.inject) {
                element.inject(this.container, "bottom");
                this.elements.push(element);
            }
        }

    });

    return UWA.namespace('dsp/component/Panel', Panel, UWA);
});



/*global define */
/*jslint nomen: true */
define("DS/W3DPassport/dsp/component/PanelV2", [
    "UWA/Core",
    "UWA/Controls/Abstract"
], function (UWA, Abstract) {
    "use strict";
    
    var PanelV2 = Abstract.extend({

        container: undefined,

        defaultOptions: {
            className: "",
            title: "",
            icon: "",
            clickIcon: null
        },

        init: function (options) {
            this._parent(options);
            this.buildSkeleton();
            this.elements = [];
        },

        /**
         *
         * @returns {undefined}
         */
        buildSkeleton: function () {
            var options = this.options;

            this.container = UWA.createElement("div", {
                "class": "uwa-panel"
            });
            this.container.addClassName(options.className);
            if (options.title) {
                this.addTitle(options.title, options.icon, options.clickIcon);
            }
        },

        /**
         *
         * @param {String} title
         * @returns {undefined}
         */
        addTitle: function (title, icon, clickIcon) {
            var titleElt,
                titleString,
                isString = typeof title === 'string',
                iconElt;

            if('link' === title.type) {
                titleElt = UWA.createElement("h1",{
                    "class": "panel-title panel-title-complex",
                    html: [{
                        tag: "a",
                        href: title.href,
                        text: title.title
                    }]});
                titleElt.inject(this.container, "top");
            } else {
                if(isString) {
                    titleString = title;
                } else {
                    titleString = title["data-dsp-i18n"];
                }
                var structure = {
                    "class": "panel-title",
                    text: UWA.i18n(titleString)
                };
                if(!isString) {
                    structure.attributes = title;
                }
                titleElt = UWA.createElement("h1",structure );
                titleElt.inject(this.container, "top");
            }
            
            if(UWA.is(icon, 'array')) {
                for(var i = 0; i < icon.length; i++){
                iconElt = UWA.createElement("span", {
                        "class":"fonticon fonticon-"+icon[i]+" icon_3dp",
                        events: {
                            click: clickIcon[i]
                        },
                        styles: {
                         "padding-left" : "5px"
                        }
                    });
                    iconElt.inject(titleElt, "bottom");
                }
            } else if(icon){
               iconElt = UWA.createElement("span",{
                   "class":"fonticon fonticon-"+icon+" icon_3dp",
                   events : {
                       click: clickIcon
                   }
               });
               iconElt.inject(titleElt, "bottom");
            }
        },
        
        setHeader: function(title){
            var header = this.container.getElement(".panel-title");
            if(header) {
                header.setText(title);
            }
        },
        
        addContentElement:  function (element) {
            if ("function" === typeof element.inject) {
                element.inject(this.container, "bottom");
                this.elements.push(element);
            }
        },
        
        removeContentElement: function (element) {
            var index = this.elements.indexOf(element);
            if(index > -1) {
                this.elements.splice(index,1);
            }
        }

    });

    return UWA.namespace('dsp/component/PanelV2', PanelV2, UWA);
});



/*global define */
/*jslint nomen: true */
define("DS/W3DPassport/dsp/component/SimplePanel", [
    "UWA/Core",
    "UWA/Controls/Abstract"
], function (UWA, Abstract) {
    "use strict";

    var SimplePanel = Abstract.extend({

        container: undefined,

        header: undefined,
        main: undefined,
        footer: undefined,
        _titleElt : undefined,//Meant to be private and do not exported
        _descriptionElt : undefined,//Meant to be private and do not exported

        defaultOptions: {
            className: "",
            title: "",
            "data-dsp-i18n": "",
            logo: true
        },

        init: function (options) {
            this._parent(options);
            this.buildSkeleton();
            this.elements = [];
        },

        buildSkeleton: function () {
            var options = this.options;

            this.container = UWA.createElement("div", {
                "class": "simple-panel"
            });
            this.container.addClassName(options.className);

            this.containerContent = UWA.createElement("div", {
                "class": "simple-panel-container-content"
            });
            this.header = UWA.createElement("div", {
                "class": "simple-panel-header"
            });
            this.main = UWA.createElement("div", {
                "class": "simple-panel-main"
            });
            this.footer = UWA.createElement("div", {
                "class": "simple-panel-footer"
            });

            if (options.logo) {
                this.addLogo(options.logo);
            }
            if (options.title) {
                this.addTitle(options.title, options.titleNls);
            }
            if (options.description) {
                this.addDescription(options.description, options.descriptionNls);
            }
            this.header.inject(this.containerContent);
            this.main.inject(this.containerContent);
            this.containerContent.inject(this.container);
            this.footer.inject(this.container);
        },

        addLogo: function (logo) {
            var elt = UWA.createElement("div", {
                "class": "panel-logo",
            });
            elt.inject(this.header);
        },

        addTitle: function (title, titleNls) {
            this._titleElt = UWA.createElement("h1", {
                "class": "panel-title",
                "html": titleNls || title,
                "data-dsp-i18n": title
            });
            //this._titleElt.setHTML(titleNls);
            this._titleElt["data-dsp-i18n"] = title;
            this._titleElt.inject(this.main);
        },

        addDescription: function (description, descriptionNls) {
            this._descriptionElt = UWA.createElement("p", {
                "class": "panel-description",
                "text": descriptionNls || description,
                "data-dsp-i18n": description
            });
            this._descriptionElt.inject(this.main);
        },

        addContentElement:  function (element) {
            if ("function" === typeof element.inject) {
                element.inject(this.main);
                this.elements.push(element);
            }
        },

        getHeader: function (){
            return this.header;
        },

        getFooter: function (){
            return this.footer;
        },
        updateTitle : function(title, titleNls){
			this.options.title = title;
			this._titleElt.setHTML(titleNls || title);
			this._titleElt.setAttribute('data-dsp-i18n', title);//For NLS conversion
			this._titleElt["data-dsp-i18n"] = title
		},
		updateDescription :  function(description, descriptionNls){
			this.options.description = description;
			this._descriptionElt.setText(descriptionNls || description);
			this._descriptionElt.setAttribute('data-dsp-i18n', description);//For NLS conversion
		}

    });

    return UWA.namespace('dsp/component/SimplePanel', SimplePanel, UWA);
});



/*global define */
/*jslint nomen: true */
define("DS/W3DPassport/dsp/component/SimpleLayout", [
    "UWA/Core",
    "UWA/Controls/Abstract"
], function (UWA, Abstract) {
    "use strict";

    var simpleLayout = Abstract.extend({

        container: undefined,

        defaultOptions: {
            className: "",
            title: "",
            "data-dsp-i18n": "",
            withBackground: true
        },

        init: function (options) {
            this._parent(options);
            this.buildSkeleton();
        },

        buildSkeleton: function () {
            var options = this.options;

            this.container = UWA.createElement("div", {
                "class": "simple-layout",
                "id": "main-content"
            });
            this.container.addClassName(options.className);
            if (options.withBackground) {
				var customBackgroundImageUrl = options.custom_background_image_url;
                var customBackground = UWA.createElement("div", {
                    "class": "simple-custom-background-container dddxp-logo-container",
                    html: [{
                        tag: "span",
                        "class": "dddxp-logo"
                    }, {
                        tag: "div",
                        "class": "simple-custom-background-image",
                        styles : customBackgroundImageUrl ? {
							"background-image" : "url("+ customBackgroundImageUrl +")",
							display : "inherit"
						} : undefined
                    }, {
                        tag: "div",
                        "class": "simple-custom-background-gradient",
                        html: [{
                            tag: "div",
                            "class": "simple-custom-background-logo"
                        }]
                    }]
                });
                this.container.addContent(customBackground);
            }
        },
        addContent: function (element) {
            if ("function" === typeof element.inject) {
                element.inject(this.container);
            }
        },
    });

    return UWA.namespace('dsp/component/SimpleLayout', simpleLayout, UWA);
});



/*global define */
/*jslint nomen: true */
define("DS/W3DPassport/dsp/component/TogglePanel", [
    "UWA/Core",
    "UWA/Controls/Abstract"
], function (UWA, Abstract) {
    "use strict";

    var togglePanel = Abstract.extend({
        container: undefined,

        defaultOptions: {
            className: "",
            title: "",
            icon: "right-dir",
            clickIcon: null,
            headerType: "p",
            headerClass: "",
            toggleContent: null,
            isOpen: false
        },

        init: function (options) {
            this._parent(options);
            this.buildSkeleton();
            this.elements = [];
        },
        
         /**
         *
         * @returns {undefined}
         */
        buildSkeleton: function () {
            var options = this.options;
            
            if(options.isOpen && options.icon === "right-dir"){
                options.icon = "down-dir";
            }

            this.container = UWA.createElement("div", {
                "class": this.options.className ? "dsp-togglepanel " + this.options.className : "dsp-togglepanel"
            });
            this.container.addClassName(options.className);
            if (options.title) {
                this.addTitle(options.title, options.icon, options.clickIcon, options.headerType, options.headerClass);
            }
            
            if (options.toggleContent){
                this.setToggleContent(options.toggleContent, options.isOpen);
            }
        },
        
        /**
         *
         * @param {String} title
         * @returns {undefined}
         */
        addTitle: function (title, icon, clickIcon, headerType, headerClass) {
            var titleElt,titleString, iconElt, headerDiv,
                isString = typeof title === 'string';
            
            headerDiv = UWA.createElement("div", {"class": "row"});
            if(icon) {
                iconElt = UWA.createElement("span",{
                    "class":"fonticon fonticon-"+icon+" icon_3dp",
                    events: {
                        click: clickIcon || this.togglePanelCallback
                    }
                });
                //iconElt.inject(titleElt, "bottom");
                iconElt.inject(headerDiv);
            }
            
            if(isString) {
                titleString = title;
            } else {
                titleString = title["data-dsp-i18n"];
            }
            var structure = {
            	"class": (headerClass ?  headerClass+" " : "") + "dsp-togglepanel-title",
                text: UWA.i18n(titleString)
            };
            if(!isString) {
                structure.attributes = title;
            }
            titleElt = UWA.createElement(headerType, structure );
            titleElt.inject(headerDiv);
            
            headerDiv.inject(this.container);
            
        },
        
        setToggleContent: function(htmlContent, openToggle) {
            var togglePanel = new UWA.createElement("div", {
                "class": openToggle ? "dsp-toggle activate" : "dsp-toggle",
                html: htmlContent,
                /*styles: (function() {
                        if(!openToggle) {
                            return  {
                                "display": "none"
                            };
                        } else {
                            return null;
                        }
                    })()*/
            });
            togglePanel.inject(this.container, "bottom");
        },

        addContentElement:  function (element) {
            if ("function" === typeof element.inject) {
                element.inject(this.container, "bottom");
                this.elements.push(element);
            }
        },
        
        removeContentElement: function (element) {
            var index = this.elements.indexOf(element);
            if(index > -1) {
                this.elements.splice(index,1);
            }
        },
        
        togglePanelCallback: function(evt) {
            var elmtParent, elmtToggle, spanElmt;
            spanElmt = evt.target;
            elmtParent = spanElmt.getClosest('.dsp-togglepanel');
            elmtToggle = elmtParent.getElement('.dsp-toggle');

            if (spanElmt.hasClassName("fonticon-down-dir")) {
                spanElmt.removeClassName("fonticon-down-dir");
                spanElmt.addClassName("fonticon-right-dir");
                elmtToggle.removeClassName("activate");
            } else {
                spanElmt.removeClassName("fonticon-right-dir");
                spanElmt.addClassName("fonticon-down-dir");
                elmtToggle.addClassName("activate");
            }

            //elmtToggle.toggle();
        }
        
    });
    
    return UWA.namespace('dsp/component/TogglePanel', togglePanel, UWA);
});

/*global define, document */
define("DS/W3DPassport/dsp/utils/cookie", [
	
], function() {
    "use strict";

    var cookie = {},
        cookies = {},
        unixEpoch = new Date(0);

    cookie.LANGUAGE = "swymlang";

    cookie.readCookie = function(name) {
        var cookieStrings,
            cookieKeyVal,
            len;

        if (!(cookies.hasOwnProperty(name))) {
            cookieStrings = document.cookie.split("; ");
            len = cookieStrings.length;
            while (0 < len) {
                len -= 1;
                cookieKeyVal = cookieStrings[len].split("=");
                cookies[cookieKeyVal[0]] = cookieKeyVal[1];
            }
        }
        return cookies[name];
    };

    cookie.writeCookie = function (name, value, expires, path, domain, secure) {
        // Secure cookie by default if unspecified
        if (secure == undefined) {
            secure = true;
        }
        document.cookie = name + "=" + escape(value) +
                (expires ? ("; Expires=" + expires.toUTCString()) : "") +
                "; Path=" + (path ?  path : "/") +
                (domain ? ("; Domain=" + domain) : "") +
                ((true === secure) ? "; Secure; SameSite=None" : "");
    };

    cookie.deleteCookie = function (name) {
        cookie.writeCookie(name, undefined, unixEpoch);
    };

    return cookie;
});


/*global define */
/**
 * @overview Language picker component
 */
 define("DS/W3DPassport/dsp/component/LanguagePicker", [
    "UWA/Core",
    "UWA/Event",
    "UWA/Controls/Abstract",
    "DS/W3DPassport/dsp/utils/cookie"
 ],
/**
 * @module LanguagePicker
 *
 * @requires UWA/Core
 * @requires UWA/Event
 * @requires UWA/Controls/Abstract
 * @requires DS/W3DPassport/dsp/utils/cookie
 *
 * @extends UWA/Controls/Abstract
 */
function (UWA, Event, Abstract, cookie) {
    "use strict";


    var LanguagePicker = Abstract.extend({
        defaultOptions: {
            className: "dsp-language-picker"
        },

        init: function (options) {
            this._parent(options);
            this.buildSkeleton();
            UWA.Element.addEvent.call(document, "click", function (event) {
                var languages = UWA.Element.getElement.call(document, ".dsp-languages");

                if (languages) {
                   languages.addClassName("closed");
                }
            });
        },

        buildSkeleton: function () {
            var that = this,
                wrapper,
                currentLanguage,
                languages;

            wrapper = UWA.createElement("div", {
                "class": "dsp-language-wrapper"
            });
            currentLanguage = UWA.createElement("div", {
                "class": "dsp-language-entry current",
                html: {
                    tag: "a",
                    href: "#"
                },
                events: {
                    click: that.onToggleLanguageList.bind(this)
                }
            });
            languages = UWA.createElement("ul", {
                "class": "dsp-languages closed",
                 events: {
                    click: that.onSelectLanguage.bind(this)
                }
            });
            currentLanguage.inject(wrapper);
            languages.inject(wrapper);
            that.elements.currentLanguage = currentLanguage;
            that.elements.languages = languages;
            that.elements.container = wrapper;
        },

        /**
         * Add a language to the list of displayed languages.
         *
         * @param {String} language A ISO 639-1 (alpha-2) code representing the language
         * @param {type} url The url to reload the page with the proper language.
         * @returns {undefined}
         */
        addLanguage: function (language, url) {
            var languageEntry = UWA.createElement("li", {
                "class": "dsp-language-entry lang-" + language,
                html: [{
                    tag: "a",
                    "class": "flag-" + language,
                    href: url,
                    text: language,
                    "data-dsp-i18n": "lang." + language
                }]
            });    
            languageEntry.inject(this.elements.languages);           
        },

        /**
         *
         * @param {type} language A ISO 639-1 (alpha-2) code representing the language
         * @returns {undefined}
         */
        setCurrentLanguage: function (language) {
            var langEntry,
                langEntries,
                len,
                anchorTag;

            langEntry = this.elements.languages.getElement(".dsp-language-entry.lang-" + language);
            if (langEntry) {
                anchorTag = this.elements.currentLanguage.getElement("a");
                anchorTag.className = langEntry.getElement("a").className;
                anchorTag.setAttributes({
                    text: language,
                    "data-dsp-i18n": "lang." + language
                });
                anchorTag.addClassName("fonticon fonticon-chevron-down");  
                langEntries = this.elements.languages.getElements(".dsp-language-entry");
                len = langEntries.length;
                while (0 < len) {
                    len -= 1;
                    langEntries[len].removeClassName("hidden");
                }
                langEntry.addClassName("hidden");
            }
        },

        /**
         * Callback called on open or close Language list actions.
         *
         * @param {Event} event
         * @returns {undefined}
         */
        onToggleLanguageList: function (event) {
            Event.stop(event);
            this.elements.languages.toggleClassName("closed");
        },

        /**
         * Callback called on language selection.
         *
         * @param {type} event
         * @returns {undefined}
         */
        onSelectLanguage: function (event) {
            var entry,
                language,
                i18n,
                cookieExpireDate;

            Event.stop(event);
            if (!(this.elements.languages.hasClassName("closed"))) {
                entry = Event.findElement(event, ".dsp-language-entry");
                language = /lang-(.+)/.exec(entry.className)[1];
                this.setCurrentLanguage(language);
                this.elements.languages.addClassName("closed");
                i18n = this.options.i18n;
                if (i18n) {
                    i18n.setLocal(language);
                    i18n.translateDocument();
                    cookieExpireDate = new Date();
                    cookieExpireDate.setFullYear(cookieExpireDate.getFullYear() + 1);
                    cookie.writeCookie(cookie.LANGUAGE, language, cookieExpireDate, undefined, this.options.domain, true);
                    if ("function" === typeof i18n.onUpdateLanguage) {
                       i18n.onUpdateLanguage(language);
                    }
                }
            }
        }
    });

    return UWA.namespace('dsp/component/LanguagePicker', LanguagePicker, UWA);
 });

/*global define*/
define("DS/W3DPassport/dsp/component/SiteHeader", [
    "UWA/Core",
    "UWA/Controls/Abstract"
], function (UWA, Abstract) {
    "use strict";
    
    var SiteHeader = Abstract.extend({
        defaultOptions: {
            className: "dsp-site-header"
        },

        init: function (options) {
            this._parent(options);
            this.buildSkeleton();
        },
        
        buildSkeleton: function () {
            var header,
                title;
        
            header = UWA.createElement("header", {
                "class": this.options.className
            });
            title = UWA.createElement("h1", {
                "class": "dsp-site-title",
                text: this.options.title
            });
            title.inject(header);
            this.elements.container = header;
        },
        
        addItem: function (item) {
            if ("function" === typeof item.inject) {
                item.inject(this.getContent());
            }
        }
    });
    
    return UWA.namespace('dsp/component/SiteHeader', SiteHeader, UWA);
});

/*global define,Object */
define("DS/W3DPassport/dsp/utils/getObjectKeys", [
	
], function () {
    "use strict";

    /**
     * Retrun an array of the keys of an object. Only return object own keys not
     * keys from the prototype chain.
     *
     * @param {Object} obj a js object
     * @returns {Array} an array of the keys of this object
     */
    return function (obj) {
        var keys,
            key;

        if ("object" === typeof obj) {
            if ("function" === typeof Object.keys) {
                keys = Object.keys(obj);
            } else {
                keys = [];
                for (key in obj) {
                    if (obj.hasOwnProperty(key)) {
                        keys.push(key);
                    }
                }
            }
        }
        return keys;
    };
});

define("DS/W3DPassport/dsp/utils/contains", [
	
], function () {
    "use strict";
    
    /**
     * 
     * @param {Array} array
     * @param {Any} elt
     * @returns {boolean}
     */
    return function (array, elt) {
        var contains = false,
            len;
        
        if (("object" === typeof array) && (array.length)) {
            if ("function" === typeof array.indexOf) {
                contains = -1 < array.indexOf(elt);
            } else {
                len = array.length;
                while ((0 < len) && !(contains)) {
                    len -= 1;
                    if (elt === array[len]) {
                        contains = true;
                    }
                }
            }
        }
        return contains;
    };
});

/*global define */
define("DS/W3DPassport/dsp/utils/removeFromArray", [
	
], function () {
    "use strict";

    return function (array, eltToRemove) {
        var indexToRemove,
            len;

        if (("object" === typeof array) && array.length) {
            if ("function" === typeof array.indexOf) {
                indexToRemove = array.indexOf(eltToRemove);
            } else {
                len = array.length;
                while (0 < len){
                    len -= 1;
                    if (eltToRemove === array[len]) {
                        indexToRemove = len;
                        break;
                    }
                }
            }
            if ((undefined !== indexToRemove) && (0 <= indexToRemove) && (array.length > indexToRemove)) {
                array.splice(indexToRemove, 1);
            }
        }
    };
});

/*global define,document */
define("DS/W3DPassport/dsp/utils/addOrUpdateUrlParams", [
    "DS/W3DPassport/dsp/utils/getObjectKeys",
    "DS/W3DPassport/dsp/utils/contains",
    "DS/W3DPassport/dsp/utils/removeFromArray"
], function(getObjectKeys, contains, removeFromArray) {
    "use strict";

    /**
     * Add or update parameters in the query part of an url.
     *
     * @param {String} url A string representing a valid url
     * @param {Object} params An Object literal of parameter keys and values
     * @returns {undefined}
     */
    return function(url, params) {
        var aTag,
            updatedUrl,
            path,
            paramsToAddOrUpdate,
            param,
            urlParams,
            keyValue,
            len,
            firstFlag;

        aTag = document.createElement("a");
        aTag.href = url;
        updatedUrl = aTag.protocol + "//" + aTag.host;
        path = aTag.pathname;
        updatedUrl = path.charAt(0) === "/" ? path : "/" + path;
        if ("" === aTag.search) {
            firstFlag = true;
            for (param in params) {
                if (params.hasOwnProperty(param)) {
                    updatedUrl += firstFlag ? "?" : "&";
                    updatedUrl += param + "=" + params[param];
                    firstFlag = false;
                }
            }
        } else {
            paramsToAddOrUpdate = getObjectKeys(params);
            urlParams = aTag.search.substr(1).split("&");
            len = urlParams.length;
            while (0 < len) {
                len -= 1;
                keyValue = urlParams[len].split("=");
                if (contains(paramsToAddOrUpdate, keyValue[0])) {
                    keyValue[1] = params[keyValue[0]];
                    urlParams[len] = keyValue.join("=");
                    removeFromArray(paramsToAddOrUpdate, keyValue[0]);
                }
            }
            updatedUrl += "?" + urlParams.join("&");
            len = paramsToAddOrUpdate.length;
            while (0 < len) {
                len -= 1;
                updatedUrl += "&" + paramsToAddOrUpdate[len] + "=" + params[paramsToAddOrUpdate[len]];
            }

        }
        return updatedUrl;
    };
});

/*global define*/
/**
 * @overview Captcha ui component
 */
define("DS/W3DPassport/dsp/component/CaptchaDisplay", [
    "UWA/Core",
    "UWA/Event",
    "UWA/Controls/Abstract",
    "DS/W3DPassport/dsp/utils/addOrUpdateUrlParams"
],
/**
 * @module CaptchaDisplay
 *
 * @requires UWA/Core
 * @requires UWA/Event
 * @requires UWA/Controls/Abstract
 * @requires DS/W3DPassport/dsp/utils/addOrUpdateUrlParams
 *
 * @extends UWA/Controls/Abstract
 */
function(UWA, Event, Abstract, addOrUpdateUrlParams) {
    "use strict";

    var CaptchaDisplay = Abstract.extend({

        init: function(options) {
            this._parent(options);
            this.buildSkeleton();
        },

        /**
         * Create dom tree for captcha UI elemets
         * @returns {undefined}
         */
        buildSkeleton: function() {
            var that = this,
                container,
                img,
                p,
                reload;

            container = UWA.createElement('div', {
                "class": "captcha-display"
            });
            img = UWA.createElement('img', {
                "class": "captcha-img",
                alt: "Captcha",
                src: this.options.captchaImgUrl
            });
            img.inject(container);
            // p = UWA.createElement('p', {
            //     "class": "captcha-reload-text",
            //     text: "If you can't read this image text, load another one.",
            //     "data-dsp-i18n": "commons.captcha.reload"
            // });
            // p.inject(container);
            reload = UWA.createElement('a', {
                "class": "captcha-reload",
                href: "#captcha-reload",
                "tabindex":"0",
                events: {
                    click: that.reloadCaptcha.bind(that)
                }
            });
            reload.inject(container);
            this.elements.container = container;
        },

        reloadCaptcha: function (event) {
            var captchaImg;

            Event.stop(event);
            captchaImg = this.elements.container.getElement(".captcha-img");
            captchaImg.src = addOrUpdateUrlParams(captchaImg.src, {
                t: Date.now(),
                reload: true
            });
        }
    });

    return UWA.namespace('dsp/component/CaptchaDisplay', CaptchaDisplay, UWA);
});



/*global define */
/**
 * @overview Page Switcher component
 */
 define("DS/W3DPassport/dsp/component/PageSwitcher", [
    "UWA/Core",
    "UWA/Event",
    "UWA/Controls/Abstract",
    "DS/W3DPassport/dsp/utils/cookie"
 ],
/**
 * @module PageSwitcher
 *
 * @requires UWA/Core
 * @requires UWA/Event
 * @requires UWA/Controls/Abstract
 * @requires DS/W3DPassport/dsp/utils/cookie
 *
 * @extends UWA/Controls/Abstract
 */
function (UWA, Event, Abstract, cookie) {
    "use strict";


    var PageSwitcher = Abstract.extend({
        defaultOptions: {
            className: "dsp-page-switcher"
        },

        init: function (options) {
            this._parent(options);
            this.buildSkeleton();
            UWA.Element.addEvent.call(document, "click", function (event) {
                var pages = UWA.Element.getElement.call(document, ".dsp-pages");

                if (pages) {
                	pages.addClassName("closed");
                }
            });
        },

        buildSkeleton: function () {
            var that = this,
                wrapper,
                currentPage,
                pages;

            wrapper = UWA.createElement("div", {
                "class": "dsp-page-switcher"
            });
            currentPage = UWA.createElement("div", {
                "class": "dsp-page-entry current",
                html: {
                    tag: "a"
                },
                events: {
                    click: that.onTogglePageList.bind(this)
                }
            });
            pages = UWA.createElement("ul", {
                "class": "dsp-pages closed",
                 events: {
                    click: that.onSelectPage.bind(this, false)
                }
            });
            currentPage.inject(wrapper);
            pages.inject(wrapper);
            that.elements.currentPage = currentPage;
            that.elements.pages = pages;
            that.elements.container = wrapper;
        },

        addPage: function (page, url) {
            var pageEntry= UWA.createElement("li", {
                "class": "dsp-page-entry page-" + page,
                html: [{
                    tag: "a",
                    "class": "flag-" + page,
                    href: url,
                    text: page,
                    "data-dsp-i18n": "commons." + page
                }]
            });
            pageEntry.inject(this.elements.pages);
        },

        setCurrentPage: function (page, redirect) {
            var pageEntry, pageElm;

            pageEntry = this.elements.pages.getElement(".dsp-page-entry.page-" + page);
            if (pageEntry) {
            	pageElm = this.elements.currentPage.getElement("a");
                pageElm.setAttributes({
                    text: page,
                    "data-dsp-i18n": "commons." + page
                });
                
                if(redirect){
                	pageElm.url = pageEntry.getElement("a").href;
                    window.location.href = pageElm.url;	
                }
            }
        },

        onTogglePageList: function (event) {
            Event.stop(event);
            this.elements.pages.toggleClassName("closed");
        },

        onSelectPage: function (event) {
            var entry,
                page,
                i18n,
                cookieExpireDate;

            Event.stop(event);
            if (!(this.elements.pages.hasClassName("closed"))) {
                entry = Event.findElement(event, ".dsp-page-entry");
                page = /page-(\w+)/.exec(entry.className)[1];
                this.setCurrentPage(page, true);
            }
        }
    });

    return UWA.namespace('dsp/component/PageSwitcher', PageSwitcher, UWA);
 });

/*global define */
define("DS/W3DPassport/dsp/UWA", [
    "UWA/Core",
    "UWA/Element",
    "UWA/Data",
    "UWA/Json",
    "UWA/Storage/Adapter/Cookies",
    "UWA/Drivers/Alone",
    "UWA/Controls/DatePicker",
    "DS/W3DPassport/dsp/component/HiddenInput",
    "DS/W3DPassport/dsp/component/PasswordInput",
    "DS/W3DPassport/dsp/component/SubmitInput",
    "DS/W3DPassport/dsp/component/InputForm",
    "DS/W3DPassport/dsp/component/Panel",
    "DS/W3DPassport/dsp/component/PanelV2",
    "DS/W3DPassport/dsp/component/SimplePanel",
    "DS/W3DPassport/dsp/component/SimpleLayout",
    "DS/W3DPassport/dsp/component/TogglePanel",
    "DS/W3DPassport/dsp/component/LanguagePicker",
    "DS/W3DPassport/dsp/component/SiteHeader",
    "DS/W3DPassport/dsp/component/CaptchaDisplay",
    "DS/W3DPassport/dsp/component/PageSwitcher"
], function (UWA) {
    "use strict";

    var inputFormCreateField,
        panelControlAddTitle,
        inputSelectBuildSkeleton,
        inputSelectSyncInput;

    UWA.Data.useJsonpRequest = false;
    UWA.Data.allowCrossOriginRequest = true;

    function addHintstoField(field, hints) {
        var hintsTag,
            hintTag,
            hint,
            len;

        if ((hints) && (0 < hints.length)) {
            hintsTag = UWA.createElement("ul", {
                "class": "hints",
                "id": "hints-for-"+field.getElement("input").name
            });
            len = hints.length;
            while (0 < len) {
                len -= 1;
                hint = hints[len];
                hintTag = UWA.createElement("li", {
                    "class" : "hint",
                    "data-dsp-i18n": hint.i18nKey,
                    "pattern" : hint.validationPattern,
                    html: hint.defaultText
                });
                if (hint.i18nFormatParams) {
                    hintTag.setAttributes({
                        "data-dsp-i18n-param": hint.i18nFormatParams.toString()
                    });
                }
                hintTag.inject(hintsTag);
            }
            hintsTag.inject(field.getElement("label"));
        }
    }

    /* -- Override UWA InputForm Control for passport i18n system ---------- */
    inputFormCreateField = UWA.dsp.component.InputForm.prototype.createField;
    UWA.dsp.component.InputForm.prototype.createField = function (fieldDef) {
        var field,
            element,
            i18nKey,
            i18nFormatParams,
            hints;
        if(fieldDef.attributes) {
        i18nKey = fieldDef.attributes["data-dsp-i18n"];
        i18nFormatParams = fieldDef.attributes["data-dsp-i18n-param"];
        hints = fieldDef.attributes.hints;
        delete fieldDef.attributes["data-dsp-i18n"];
        delete fieldDef.attributes.hints;
        } else {
            i18nKey = "";
            hints = "";
        }
        field = inputFormCreateField.call(this, fieldDef);
        element = field.getElement(".label")
            || field.getElement(".uwa-submit")
            || field.getElement(".uwa-button");
        if (element && i18nKey) {
            element.setAttribute("data-dsp-i18n", i18nKey);
            if(i18nFormatParams){
                element.setAttribute("data-dsp-i18n-param", i18nFormatParams);
            }
        }
        addHintstoField(field, hints);
        return field;
    };

    UWA.dsp.component.InputForm.prototype.inputFactory.dateTime = function (options) {
        return new UWA.Controls.DatePicker(options);
    };

    UWA.dsp.component.InputForm.prototype.inputFactory.hidden = function (options) {
        return new UWA.Controls.Input.Hidden(options);
    };

    UWA.dsp.component.InputForm.prototype.inputFactory.password = function (options) {
        return new UWA.Controls.Input.Password(options);
    };

    UWA.dsp.component.InputForm.prototype.inputFactory.submit = function (options) {
        return new UWA.Controls.Input.Submit(options);
    };

    /* -- Override UWA Panel Control -- */
    panelControlAddTitle = UWA.dsp.component.Panel.prototype.addTitle;
    UWA.dsp.component.Panel.prototype.addTitle = function (title) {
        panelControlAddTitle.call(this, title);
        var panelTitle = this.container.getElement(".panel-title:not(.panel-title-complex)");
        if(panelTitle && !panelTitle.getAttribute("data-dsp-i18n")) {
            panelTitle.setAttribute("data-dsp-i18n", title);
        }
    };

    inputSelectSyncInput = UWA.Controls.Input.Select.prototype.syncInput;
    UWA.Controls.Input.Select.prototype.syncInput = function () {
        var input = this.elements.input,
            options,
            option,
            name,
            len;
        if(!input.hasAttribute("notranslate")) {
            if ("function" === typeof input.querySelectorAll) {
                options = input.querySelectorAll("option:not([data-dsp-i18n])");
            } else {
                options = input.getElementsByTagName("option");
            }
            if(input.hasAttribute("nls-prefix")) {
                name = input.getAttribute("nls-prefix");
            } else {
                name = /data\[(.+)\]/.exec(input.name)[1];
            }
            len = options.length;
            while (0 < len) {
                len -= 1;
                option = options[len];
                if (!(option.hasAttribute("data-dsp-i18n"))) {
                    if (option.value) {
                        option.setAttribute("data-dsp-i18n", name +'.'+ option.value);
                    } else {
                        option.setAttribute("data-dsp-i18n", name +'.'+ "default");
                    }
                }
            }
        }
        inputSelectSyncInput.call(this);
    };

    return UWA;
});

/*global define */
define("DS/W3DPassport/dsp/i18n/Ii18n", [
	
], function () {
    "use strict";

    /** 
     * An interface form the I18n implementations.
     * 
     * @interface
     * @constructor
     */
    var Ii18n = function () {
        this.locale = undefined;
    };

    /**
     * A method to initialiaze implementation configuration details, default
     * locale ...
     * 
     * @param {Object} options 
     * @returns {undefined}
     */
    Ii18n.prototype.init = function (options) {};

    /**
     * Change the current locale. Allow implementations to handle dynamic
     * language loading.
     * 
     * @param {String} locale
     * @returns {undefined}
     */
    Ii18n.prototype.setLocal = function (locale) {};

    /**
     * Retreive the translated message for a given key. It can take a optional
     * array parameter for parametrized string.
     * 
     * @param {String} key The translation key
     * @param {Array} params The parameters to be replaced in a parametrized string
     * @returns {String} The translated message.
     */
    Ii18n.prototype.translate = function (key, params) {};

    /**
     * Translate the all the translation keys the document contains.
     * 
     * @returns {undefined}
     */
    Ii18n.prototype.translateDocument = function () {};

    return Ii18n;
});

/*global define */
/*jslint browser: true, nomen: true */
define("DS/W3DPassport/dsp/i18n/I18nDspImpl", [
    "DS/W3DPassport/dsp/i18n/Ii18n",
    "DS/W3DPassport/dsp/UWA",
    "DS/W3DPassport/dsp/utils/cookie",
    "DS/W3DPassport/dsp/utils/contains",
], function (Ii18n, UWA, cookie, contains) {
    

    var I18nDspImpl,
        _retryWait = 42;

    /* -- Private ----------------------------------------------------------- */

    /**
     * Call json rest service on iam-webapp to retrieve a dictionary object.
     *
     * @param {String} url Url for the dictionary resource.
     * @param {String} locale A representation of the language (ex: "en", "en_us").
     * @param {Object} dicos The dictionary list to populate.
     * @returns {undefined}
     */
    function fetchLanguage(url, locale, dicos) {
        UWA.Data.request(url + "?ts=" + getVersion(), {
            type: "json",
            proxy: false,
            onComplete: function (data) {
                dicos[locale] = data;
            }
        });
    }
    
    function getVersion() {
        if (this.version === undefined) {
            this.version = new Date().setHours(0, 0, 0, 0);
        }
        let metaTag = document.getElementsByName('application-name')[0];
        if (metaTag !== undefined) {
            this.version = metaTag.getAttribute('data-version') || this.version;
        }
        return this.version;
    }

    /**
     * Format a string by replacing placeholders with given parameters. The
     * placeholder are the one used in properties files with brackets notation.
     *
     * @param {String} str A parametrized string
     * @param {String} params
     * @returns {String} The formated string
     */
    function format(str, params) {
        var args = params.split(",");
		args = args.map(function(elt) {
			return elt.replace(/#######COMMA#######/g,",");
		});
        return str.replace(/\{(\d+)\}/g, function() {
            return args[arguments[1]];
        });
    }
    /**
     * Find a translation for a key in a dictionnary. Format the translation
     * string with the parameters if some are given.
     *
     * @param {Object} dictionary
     * @param {String} key
     * @param {String} params
     * @returns {String} the translation or undefined if it is not found.
     */
    function translateKey(dictionary, key, params) {
        var translation;

        if (dictionary.hasOwnProperty(key)) {
            if (params === undefined) {
                translation = dictionary[key];
            } else {
                translation = format(dictionary[key], params);
            }
        }
        return translation;
    }

    function setLabel(elt, label) {
        var input;

        if (elt.match("input[type=\"submit\"]")) {
            elt.setAttributes({
                value: label
            });
        } else if (elt.match(".label")) {
            elt.setHTML(label);
            input = elt.getParent().getElement("input");
            //don't want placeholders on registerform
            if (input && input.hasAttribute("placeholder") && (document.getElementsByClassName("register-form").length == 0)) {
                input.placeholder = label;
            }
        } else {
            elt.setHTML(label);
        }
    }

    function syncSelectInput() {
        var elts = UWA.Element.getElements.call(document.body, "select"),
            i = elts.length;

        while (i > 0) {
            i -= 1;
            UWA.Event.dispatchEvent(elts[i], "keydown");
        }
    }
    
	/* Function to order the country field by alphabetic order  */
    function orderSelectInput(listOption, selectedValue) {
		var opt =1;
    	var divSelectOld = UWA.Element.getElement.call(document.body, ".uwa-select");  
    	if(divSelectOld.hasClassName("required")){
	        var requiredField = divSelectOld.hasClassName("required")? "required": "";
	        var disabledField = divSelectOld.hasClassName("disabled")? " disabled": "";
	    	var parent = divSelectOld.parentNode ;
	    	divSelectOld.destroy(); 	
	    	// By Pass for destroy() bug: after .destroy all option become selected true...
	    	for (opt = 1; opt < listOption.length; opt++) {
	    		if(listOption[opt].value == selectedValue){
					listOption[opt].selected = true; 
				}else{
					listOption[opt].selected = false ;
				}
			}    	
	    	// Create the select element, translated and sorted by alphabetic order
	        var selectCountries = new UWA.Controls.Input.Select({"className": requiredField, attributes: {name: 'data[country]', "required": requiredField, "disabled": disabledField, "placeholder": ""}});        
	        selectCountries.putOptions(listOption);   
	    	selectCountries.inject(parent);
    	}
    }
	

    /* -- Public ------------------------------------------------------------ */

    /**
     *
     * @constructor
     * @implements {Ii18n}
     */
    I18nDspImpl = function () {
        Ii18n.call(this);
        this.dataAttrKey = "data-dsp-i18n";
        this.dataAttrParamKey = "data-dsp-i18n-param";
        this.i18nApiUrl = undefined;
        this.locale = undefined;
        this.dictionaries = {};
        this.initialized = false;
        this.version = new Date().setHours(0, 0, 0, 0); /* safe default */
    };

    I18nDspImpl.prototype = new Ii18n();
    I18nDspImpl.prototype.constructor = I18nDspImpl;

    /**
     * @param {Object} options A hashmap of option properties
     * @returns {undefined}
     * @override
     */
    I18nDspImpl.prototype.init = function (options) {
        var language,
            browserLocale,
            i18nConfig = options.i18nConfig || {};

        this.i18nApiUrl = options.i18nApiUrl;
        this.initialized = true;
        if (options.browserLocale) {
            browserLocale = options.browserLocale.split("_")[0];
        }
        language = cookie.readCookie("swymlang") || options.language || browserLocale;
        if (!contains(i18nConfig.supportedLanguages, language)) {
           language = i18nConfig.defaultLanguage || "en";
        }
        if (language !== "en") {
            this.setLocal("en"); // Init fallback
        }
        this.setLocal(language);
    };

    /**
     * @param {String} locale A representation of the language (ex: "en", "en_us")
     * @throws {Error} When the object has not been initialized.
     * @returns {undefined}
     * @override
     */
    I18nDspImpl.prototype.setLocal = function (locale) {
        if (!(this.initialized)) {
            throw new Error("I18nDspImpl object has not be initialized");
        }
        this.locale = locale;
        if (undefined === this.dictionaries[locale]) {
            fetchLanguage(this.i18nApiUrl + "/" + locale, locale, this.dictionaries);
        }
    };

    /**
     * Retrun the translation for a given key with optional parameters for
     * parametrized key. This method suppose that the dictionary for the current
     * locale is ready otherwise it will return translation key. For asynchronous
     * behaviour use translateDocument().
     *
     * @param {String} key Translation key.
     * @param {String} params Values for parametrized translation strings.
     * @throws {Error} When the object has not been initialized.
     * @returns {String} Return the translation string or undefined if it was
     *                   not or the translation key if dictionary was not ready.
     * @override
     */
    I18nDspImpl.prototype.translate = function (key, params) {
        var dico,
            trans;

        if (!(this.initialized)) {
            throw new Error("I18nDspImpl object has not be initialized");
        }
        dico = this.dictionaries[this.locale];
        if (dico && dico.size > 0 && dico.entries[key]) {
            trans = translateKey(dico.entries, key, params);
        } else if (this.dictionaries.en) {
            trans = translateKey(this.dictionaries.en.entries, key, params);
        }
        if (trans === undefined) {
            trans = key;
        }
        return trans;
    };

    /**
     * @throws {Error} When the object has not been initialized.
     * @returns {undefined}
     * @override
     */
	I18nDspImpl.prototype.translateDocument = function () {
		var that = this,
		elts,
		elt,
		key,
		param,
		selectedValue,
		i;
		
		var countryOptionTranslated = [] ;

		if (!(this.initialized)) {
			throw new Error("I18nDspImpl object has not be initialized");
		}
		// If dictionary is not ready yet wait for the download and retry.
		if (undefined === this.dictionaries[this.locale]) {
			setTimeout(function () {
				that.translateDocument();
			}, _retryWait);
		} else {
			
			
			elts = UWA.Element.getElements.call(document.body, "[" + this.dataAttrKey + "]");
			i = elts.length;
			var defaultCountryElt;
			while (0 < i) {

				i -= 1;
				elt = elts[i];
				key = elt.getAttribute(this.dataAttrKey);
				param = elt.getAttribute(this.dataAttrParamKey);

				if (param) {
					setLabel(elt, this.translate(key, param));
				} else {
					setLabel(elt, this.translate(key));	
					var isDefaultValue = "country.default" === elts[i].getAttribute(this.dataAttrKey);
					//Store elt type options country in a array to sort it after
					if ( (typeof elts[i] != 'undefined') && (elts[i].getAttribute(this.dataAttrKey).indexOf("country.") != -1) && (elts[i].getAttribute(this.dataAttrKey).indexOf("country.label") == -1) ) {
						setLabel(elt, this.translate(key));
						if(isDefaultValue) {
							defaultCountryElt = elt;
						} else {
							countryOptionTranslated.push(elt);
						}
						if(elt.selected == true){
							selectedValue = elt.value;
						}
					}
				}

			}
			
			//Sort the array in alphabetic order
			if (typeof countryOptionTranslated !== 'undefined' && countryOptionTranslated.length > 0) {

				countryOptionTranslated.sort(function(a, b){
					if(a.text < b.text) return -1;
					if(a.text > b.text) return 1;
					return 0;
				})
				countryOptionTranslated.unshift(defaultCountryElt);
				//Empty select elt of countries and re-create it in correct order.
				orderSelectInput(countryOptionTranslated, selectedValue);					
			}
			syncSelectInput();					

		}


	};


	return I18nDspImpl;
});

/*global define */
define("DS/W3DPassport/dsp/i18n/i18n", [
    "DS/W3DPassport/dsp/i18n/I18nDspImpl"
], function (I18n) {
    "use strict";

    return new I18n();
});

/*global define */
define("DS/W3DPassport/dsp/layout/SinglePanelLayout", [
    "DS/W3DPassport/dsp/UWA",
    "UWA/Controls/Abstract"
], function (UWA, Abstract) {
    "use strict";

    var SinglePanelLayout = Abstract.extend({
        header: undefined,
        panels: [],

        init: function (options) {
            this._parent(options);
        },

        setHeader: function (header) {
            this.header = header;
        },

        setPanel: function (panel, classname) {
            this.panels = [];
            this.addPanel(panel, classname);
        },

        addPanel: function(panel, classname){
            panel.getContent().addClassName("single-panel");
            if(classname){
                panel.getContent().addClassName(classname);
            }
            this.panels.push(panel);
        },

        inject: function (container) {
            if (this.header) {
                this.header.getContent().inject(container);
            }
            // ES5 for IE11
            [].forEach.call(this.panels, function(panel) {
                if (panel) {
                    panel.getContent().inject(container);
                }
            });
        }
    });

    return SinglePanelLayout;
});

/*global define */
define("DS/W3DPassport/dsp/layout/SinglePanelLayoutV2", [
    "DS/W3DPassport/dsp/UWA",
    "UWA/Controls/Abstract"
], function (UWA, Abstract) {
    "use strict";

    var SinglePanelLayout =  Abstract.extend({
        header: undefined,
        panel: undefined,
        className: undefined,
        id: undefined,

        init: function (options) {
            this._parent(options);
        },

        setHeader: function (header) {
            this.header = header;
        },

        setPanel: function (panel) {
            var classname, id;
            classname = this.options.className ? this.options.className : "single-panel";
            this.panel = panel;
            
            this.panel.getContent().addClassName(classname);

            if(this.options.id){
                this.panel.getContent().setAttribute("id", this.options.id);
            }
        },

        inject: function (container) {
            if (this.header) {
                this.header.getContent().inject(container);
            }
            if (this.panel) {
                this.panel.getContent().inject(container);
            }
        }
    });

    return SinglePanelLayout;
});

/*global define */
define("DS/W3DPassport/dsp/utils/addCaptchaToFields", [
	
], function () {
    "use strict";

    return function (config, fields) {
        if (config.needsCaptcha && config.captchaType === "legacyCaptcha") {
            fields.push({
                className: "captcha required",
                type: "text",
                label: "Type the characters you see above",
                attributes: {
                    name: "captcha",
                    "data-dsp-i18n": "field.captcha.label",
                    required: "required",
                    "spellcheck": "false",
                    "autocomplete": "off",
                    "autocorrect": "off",
                    "autocapitalize": "off"
                }
            });
        }
    };
});


/*global define */
define("DS/W3DPassport/dsp/utils/addCsrfToFields", [
	
], function() {
	"use strict";

	return function(config, fields) {
		if (config.csrfTokenValue && config.csrfTokenName) {
			fields.push({
				className : "hidden",
				type : "hidden",
				value : config.csrfTokenValue,
				attributes : {
					name : config.csrfTokenName,
				}
			});
		}
	};
});

/*global define */
define("DS/W3DPassport/dsp/utils/addMessagesToPanel", [
    "DS/W3DPassport/dsp/UWA"
], function (UWA) {
    "use strict";

    function createMsgLists(msgs, type) {
        var msgsTag,
            msgTag,
            hrefTag,
            i18nKey,
            hrefLink,
            len,
            i;

        msgsTag = UWA.createElement("ul", {
            "class": type + "-messages"
        });
        len = msgs.length;
        for (i = 0; i < len; i += 1) {
        	var msg = msgs[i];
        	hrefLink = msgs[i].hrefLink;
        	if((undefined !== hrefLink) && (null !== hrefLink) && hrefLink.length != 0){
        		msgTag = UWA.createElement("li", {
        			"class": type + "-message",
                     html: {
                         tag: "a",
                         text: msgs[i].defaultMessage,
                         href: msgs[i].hrefLink
                     }
        		});
        		
        	} else {
                msgTag = UWA.createElement("li", {
                    "class": type + "-message",
                    text: msgs[i].defaultMessage
                });
                

        	}
        	i18nKey = msgs[i].i18nKey;
            if ((undefined !== i18nKey) && (null !== i18nKey)) {
                msgTag.setAttributes({
                    "data-dsp-i18n" : i18nKey
                });
            }
            if(msg.parameters) {
                msgTag.setAttributes({
                    "data-dsp-i18n-param" : msg.parameters.join(',')
                });
            }
            
            msgTag.inject(msgsTag);
        }
        return msgsTag;
    }

    return function (config, panel) {
        var errorMsgs,
            notificationMsgs,
            msgsElt;

        errorMsgs = config.errorMsgs;
        if (errorMsgs && "object" === typeof errorMsgs && errorMsgs.length) {
            msgsElt = createMsgLists(errorMsgs, "error");
            panel.addContentElement(msgsElt);
        }
        notificationMsgs = config.notificationMsgs;
        if (notificationMsgs && "object" === typeof notificationMsgs && notificationMsgs.length) {
            msgsElt = createMsgLists(notificationMsgs, "notification");
            panel.addContentElement(msgsElt);
        }
    };
});

/*global define */
define("DS/W3DPassport/dsp/utils/createLanguagePicker", [
    "DS/W3DPassport/dsp/UWA"
], function (UWA) {
    "use strict";

    var dsp = UWA.dsp;

    return function(i18n, domain) {
        var languagePicker;
        languagePicker = new UWA.dsp.component.LanguagePicker({
            i18n: i18n, domain: domain
        });
        languagePicker.addLanguage("en", "#");
        languagePicker.addLanguage("fr", "#");
        languagePicker.addLanguage("de", "#");
        languagePicker.addLanguage("ja", "#");
        languagePicker.addLanguage("ko", "#");
        languagePicker.addLanguage("pt-BR", "#");
        languagePicker.addLanguage("ru", "#");
        languagePicker.addLanguage("zh", "#");
        languagePicker.addLanguage("it", "#");
        languagePicker.addLanguage("es", "#");
        languagePicker.addLanguage("pl", "#");
        languagePicker.addLanguage("cs", "#");
        languagePicker.addLanguage("zh-TW", "#");
        languagePicker.addLanguage("tr", "#");
        languagePicker.setCurrentLanguage(i18n.locale);

        return languagePicker;
    };
});

/*global define */
define("DS/W3DPassport/dsp/utils/createPageSwitcher", [
    "DS/W3DPassport/dsp/UWA"
], function (UWA) {
    "use strict";

    var dsp = UWA.dsp;

    return function(i18n, config) {
        var pageSwitcher;
        var isDsConnectProfile = (window.self !== window.top);
        pageSwitcher = new UWA.dsp.component.PageSwitcher({
            i18n: i18n, domain: config.cookieDomain
        });
        
        Object.keys(config.pages).forEach(function (key) {
        	
        	if(key == "twoStepAuth" && !isDsConnectProfile && true !== config.embedMode){
        		pageSwitcher.addPage(key, config.pages[key]);
        	} else if (key != "twoStepAuth"){
        		pageSwitcher.addPage(key, config.pages[key]);
        	}
        });
        
        pageSwitcher.setCurrentPage("myProfile", false);

        return pageSwitcher;
    };
});

/*global define */
define("DS/W3DPassport/dsp/DSP", [
    "DS/W3DPassport/dsp/UWA",
    //"DS/W3DPassport/dsp/UIKIT",
    //"DS/W3DPassport/dsp/W3DXComponents",
    "DS/W3DPassport/dsp/i18n/i18n",
    "DS/W3DPassport/dsp/layout/SinglePanelLayout",
    "DS/W3DPassport/dsp/layout/SinglePanelLayoutV2",
    "DS/W3DPassport/dsp/utils/addCaptchaToFields",
    "DS/W3DPassport/dsp/utils/addCsrfToFields",
    "DS/W3DPassport/dsp/utils/addMessagesToPanel",
    "DS/W3DPassport/dsp/utils/addOrUpdateUrlParams",
    "DS/W3DPassport/dsp/utils/createLanguagePicker",
    "DS/W3DPassport/dsp/utils/createPageSwitcher",
    "DS/W3DPassport/dsp/utils/cookie"
], function () {
    // Empty function that will be populated by optimization process with the
    // dependencies above.
});

