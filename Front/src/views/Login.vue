<template>
    <div id="wrap">
        <header>Portal-IT</header>
        <main>
            <article>
                <div id="login-box">
                    <form id="login-form">
                        <div id="id-input-box">
                            <input
                                id="id-input"
                                type="text"
                                placeholder="아이디를 입력하세요."
                            />
                        </div>
                        <div id="pw-input-box">
                            <input
                                id="pw-input"
                                type="password"
                                placeholder="비밀번호를 입력하세요."
                            />
                        </div>
                        <button id="login-submit" type="submit">로그인</button>
                    </form>

                    <div class="divider">
                        <hr />
                        <span>또는</span>
                        <hr />
                    </div>

                    <button id="signup-button">회원가입</button>
                </div>
            </article>
        </main>
        <footer></footer>
    </div>
</template>
