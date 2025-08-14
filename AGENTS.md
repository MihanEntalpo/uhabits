# Agent Instructions

## Environment setup

*Install JDK 17*
```sh
curl -L -o /tmp/jdk17.tar.gz https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.8%2B7/OpenJDK17U-jdk_x64_linux_hotspot_17.0.8_7.tar.gz
sudo tar -xzf /tmp/jdk17.tar.gz -C /opt
export JAVA_HOME=/opt/jdk-17.0.8+7
export PATH="$JAVA_HOME/bin:$PATH"
```

*Trust the MITM proxy certificate*
```sh
sudo /opt/jdk-17.0.8+7/bin/keytool -import -trustcacerts -file /etc/ssl/certs/envoy-mitmproxy-ca-cert.pem -alias envoy-mitmproxy -keystore "$JAVA_HOME/lib/security/cacerts" -storepass changeit -noprompt
```

*Run tests*
```sh
JAVA_HOME=/opt/jdk-17.0.8+7 ./gradlew uhabits-core:test --no-daemon --console=plain
```

*Android SDK*

Install the Android SDK command-line tools and required platforms, then set `ANDROID_SDK_ROOT` to that directory to build Android modules.
