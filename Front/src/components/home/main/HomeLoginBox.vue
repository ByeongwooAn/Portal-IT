<template>
    <div id="login-box">
        <div id="login-group">
            <RouterLink to="/login" id="login-button">로그인</RouterLink>
            <div id="auth-links">
                <a>아이디 찾기</a>
                <span>|</span>
                <a>비밀번호 찾기</a>
                <span>|</span>
                <a>회원가입</a>
            </div>
        </div>
    </div>
</template>

<style scoped>
#login-box {
    width: 460px;
    height: 184px;
    border: solid 1px #e3e5e8;
    border-radius: 10px;
    align-content: center;
}

#login-group {
    width: 416px;
    margin: 0 auto;
}

#login-button {
    display: block;
    width: 415px;
    height: 65px;
    background-color: #2a54fb;
    border-radius: 5px;
    border: none;
    font-size: 32px;
    font-weight: bold;
    color: white;
    text-align: center;
    align-content: center;
}

#login-button:active {
    background-color: #0f3cf0;
}

#login-button > a {
    width: 100%;
    height: 100%;
}

#auth-links {
    width: 300px;
    margin: 0 auto;
    margin-top: 10px;
}

#auth-links > a,
#auth-links > span {
    color: #808080;
    margin-left: 10px;
}
</style>
