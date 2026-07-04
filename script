function copy(id) {
    const text = document.getElementById(id).innerText;

    navigator.clipboard.writeText(text).then(() => {
        alert("✅ Address copied successfully!");
    }).catch(() => {
        alert("❌ Copy failed.");
    });
}

function showQR(type){

    let address="";

    if(type==="btc"){
        address="bc1q0qacgswtxjkrtqmw7tpuj387el3r4lyj4s2mfz";
    }

    if(type==="eth"){
        address="0xcb5a380102d49ad4a8af619c65c50d6a22c7b77c";
    }

    if(type==="usdt"){
        address="0xcb5a380102d49ad4a8af619c65c50d6a22c7b77c";
    }

    const box=document.getElementById(type+"qr");

    if(box.innerHTML!=""){
        box.innerHTML="";
        return;
    }

    box.innerHTML=
    `<img src="https://api.qrserver.com/v1/create-qr-code/?size=220x220&data=${encodeURIComponent(address)}" alt="QR Code">`;

}