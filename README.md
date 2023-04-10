
<!DOCTYPE html>

<html>

<head>
    <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.3.1/css/bootstrap.min.css"
        integrity="sha384-ggOyR0iXCbMQv3Xipma34MD+dH/1fQ784/j6cY/iJTQUOhcWr7x9JvoRxT2MZw1T" crossorigin="anonymous">
    <link rel="icon" type="image/png" href="/favicon.png" />
    <link rel="stylesheet" href="style.css">
    <script src="script.js"></script>

    <title>Rammerhead Proxy</title>
</head>

<body>
    <header>
        <img src="logo.png" />
        <h1>Rammerhead Proxy</h1>
    </header>
    <div class="container mb-5">
        <p class="mt-3 mb-3 font-weight">Join the <a href="https://discord.gg/VNT4E7gN5Y">Discord server</a> for updates
            or just chat about life</p>
        <p class="mb-0 font-weight-bold">Notice: inactive sessions will be deleted after 3 days.</p>
        <p class="mb-3 font-weight-bold">Notice 2: Treat every session id like an isolated incognito browser that
            belongs only to you. DO NOT SHARE THE SESSION ID. All logins that you make with the session id will be saved
            in that session. Anyone that has your session id or session url CAN ACCESS your logged in sites.</p>
        <p class="mb-3 font-weight-bold text-danger" id="error-text" style="display: none">Error: some text</p>
        <div class="input-group mb-2" id="password-wrapper" style="display: none">
            <div class="input-group-prepend">
                <span class="input-group-text">Enter password</span>
            </div>
            <input type="password" class="form-control" id="session-password"
                placeholder="Password is given by host of this site.">
        </div>
        <div class="input-group mb-2">
            <div class="input-group-prepend">
                <span class="input-group-text">Enter URL</span>
            </div>
            <input type="text" class="form-control" id="session-url" placeholder="https://www.google.com/">
            <div class="input-group-append">
                <button class="btn btn-success" id="session-go">Go!</button>
            </div>
        </div>
        <div class="input-group mb-4">
            <div class="input-group-prepend">
                <span class="input-group-text">Session ID</span>
            </div>
            <input readonly type="text" class="form-control disable-text" id="session-id"
                placeholder="click on 'Create new session ID' or 'Fill in existing session ID' from below">
            <div class="input-group-append">
                <button class="btn btn-secondary" id="session-create-btn" type="button">Create new session ID</button>
            </div>
        </div>
        <button class="btn btn-outline-secondary" id="session-advanced-toggle">Show advanced options</button>
        <div class="mt-2 mb-4" id="session-advanced-container" style="display: none">
            <div class="form-check mb-1">
                <input class="form-check-input" type="checkbox" value="" id="session-shuffling" checked>
                <label class="form-check-label" for="session-shuffling">Enable URL Shuffling</label>
            </div>
            <div class="input-group mb-3">
                <div class="input-group-prepend">
                    <span class="input-group-text">HTTP Proxy</span>
                </div>
                <input type="text" class="form-control" id="session-httpproxy"
                    placeholder="http://username:password@proxyipaddress:proxyport">
            </div>
        </div>
    </div>
    <div class="row justify-content-center m-0">
        <table class="table w-75 table-striped table-bordered">
            <thead>
                <tr>
                    <th>Session ID</th>
                    <th>Created on</th>
                </tr>
            </thead>
            <tbody>
            </tbody>
        </table>
    </div>
</body>

</html>
