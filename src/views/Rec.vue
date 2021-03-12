<template>
<div class="pure-g">

    <!-- Video area -->
    <div class="pure-u-2-3" id="video-container">
        <video id="their-video" autoplay></video>
        <video id="my-video" muted="true" autoplay></video>
    </div>

    <!-- Steps -->
    <div class="pure-u-1-3">
        <h2>SkyWay Video Chat</h2>

        <p>Your id: <span id="my-id">...</span></p>
        <p>Share this id with others so they can call you.</p>
        <h3>Make a call</h3>
        <form id="make-call" class="pure-form">
            <input type="text" placeholder="Call user id..." id="callto-id">
            <button href="#" class="pure-button pure-button-success" type="submit">Call</button>
        </form>
        <form id="end-call" class="pure-form">
            <p>Currently in call with <span id="their-id">...</span></p>
            <button href="#" class="pure-button pure-button-success" type="submit">End Call</button>
        </form>
    </div>
</div>

</template>

<style>
.pure-button-success,
.pure-button-error,
.pure-button-warning,
.pure-button-secondary {
    color: white;
    border-radius: 4px;
    text-shadow: 0 1px 1px rgba(0, 0, 0, 0.2);
}
.pure-button-success {
    background: rgb(28, 184, 65); /* this is a green */
}
.pure-button-error {
    background: rgb(202, 60, 60); /* this is a maroon */
}
.pure-button-warning {
    background: rgb(223, 117, 20); /* this is an orange */
}
.pure-button-secondary {
    background: rgb(66, 184, 221); /* this is a light blue */
}





*, *:before, *:after {
    -moz-box-sizing: border-box; -webkit-box-sizing: border-box; box-sizing: border-box;
}

#my-video {
    margin-top: 15px;
    width: 280px;
    height: auto;
    background-color: #eee;
}

#their-video {
    width: 100%;
    height: 75%;
    max-height: 480px;
    background-color: #eee;
}

#video-container {
    padding: 25px;
    text-align: center;
}

#end-call {
    display: none;
}

#my-id {
    font-weight: bold;
}
</style>