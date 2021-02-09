<template>
  <Layout :sidebar="false">
<div class="content">
		<h2>{{ this.description }}</h2><br>
		<h3 id="configuration"><a href="#configuration" aria-hidden="true"><span class="icon icon-link"></span></a><u>Configuration</u></h3>
			<p class="conf">
				<strong>DNS-over-TLS:</strong> <code class="language-text">tls://dns.arapurayil.com</code><br>
				<strong>DNS-over-HTTPS:</strong> <code class="language-text">https://dns.arapurayil.com/dns-query</code><br>
				<strong>DNS-over-QUIC:</strong> <code class="language-text">quic://dns.arapurayil.com:784</code><br>
        <strong>DNSCrypt (IPv4):</strong> <code class="language-text">sdns://AQMAAAAAAAAAEDMuNy4xNzYuMTIzOjg0NDMggyXjcEBxUFeQc2O5FaBzadiWC6vE6NTTQP84IY-Xfl8dMi5kbnNjcnlwdC1jZXJ0LmFyYXB1cmF5aWwtaW4</code><br>
        <strong>DNSCrypt (IPv6):</strong> <code class="language-text">sdns://AQMAAAAAAAAALFsyNDA2OmRhMWE6YzU5OmFlMDA6MjBmOmRiZjU6YTEyYzo1YWZiXTo4NDQzIIMl43BAcVBXkHNjuRWgc2nYlgurxOjU00D_OCGPl35fHTIuZG5zY3J5cHQtY2VydC5hcmFwdXJheWlsLWlu</code><br>
		<h3 id="implementations"><a href="#implementations" aria-hidden="true"><span class="icon icon-link"></span></a><u>Implementations</u></h3>
			<p>
			<h4 id="android"><a href="#android" aria-hidden="true"><span class="icon icon-link"></span></a>Android</h4>
				<ul>
					<li>Android 9 supports <code class="language-text">DNS-over-TLS</code> natively.
						To configure it, go to <em>Settings → Network &amp; internet → Advanced → Private DNS</em> and enter <code class="language-text">dns.arapurayil.com</code>there.</li>
					<li><a href="https://getintra.org/" title="Intra" target="_blank" rel="nofollow noopener noreferrer">Intra</a> adds <code class="language-text">DNS-over-HTTPS</code> support to Android.</li>
					<li><a href="https://adguard.com/adguard-android/overview.html" title="AdGuard for Android" target="_blank" rel="nofollow noopener noreferrer">AdGuard for Android</a> supports <code class="language-text">DNS-over-HTTPS</code> and <code class="language-text">DNS-over-TLS</code>.</li>
				</ul>
			<h4 id="ios"><a href="#ios" aria-hidden="true"><span class="icon icon-link"></span></a>iOS</h4>
				<ul>
					<li>
						<p>On an iOS 14 or macOS Big Sur device you can download special '.mobileconfig' file that adds <code class="language-text">DNS-over-HTTPS</code> or <code class="language-text">DNS-over-TLS</code> servers to the DNS settings.</p>
						<ul>
							<li><a href="/apple/dot.mobileconfig" title="Download .mobileconfig for DNS-over-TLS" target="_blank" rel="nofollow noopener noreferrer">Download .mobileconfig for DNS-over-TLS</a></li>
							<li><a href="/apple/doh.mobileconfig" title="Download .mobileconfig for DNS-over-HTTPS" target="_blank" rel="nofollow noopener noreferrer">Download .mobileconfig for DNS-over-HTTPS</a></li>
						</ul>
						</li>
						<li><a href="https://itunes.apple.com/app/id1452162351" title="DNSCloak" target="_blank" rel="nofollow noopener noreferrer">DNSCloak</a> supports <code class="language-text">DNS-over-HTTPS</code>.</li>
					<li><a href="https://adguard.com/adguard-ios/overview.html" title="AdGuard for iOS" target="_blank" rel="nofollow noopener noreferrer">AdGuard for iOS</a> supports <code class="language-text">DNS-over-HTTPS</code> and <code class="language-text">DNS-over-TLS</code> setup.</li>
				</ul>
			</p>
			<h3 id="other-implementations"><a href="#other-implementations" aria-hidden="true"><span class="icon icon-link"></span></a><u>Other implementations</u></h3>
				<ul>
					<li><a href="https://github.com/AdguardTeam/AdGuardHome" title="AdGuard Home" target="_blank" rel="nofollow noopener noreferrer">AdGuard Home</a> can be a secure DNS client on any platform.</li>
					<li><a href="https://github.com/AdguardTeam/dnsproxy" title="dnsproxy" target="_blank" rel="nofollow noopener noreferrer">dnsproxy</a> supports all known secure DNS protocols.</li>
					<li><a href="https://github.com/jedisct1/dnscrypt-proxy" title="dnscrypt-proxy" target="_blank" rel="nofollow noopener noreferrer">dnscrypt-proxy</a> supports <code class="language-text">DNS-over-HTTPS</code>.</li>
					<li><a href="https://support.mozilla.org/kb/firefox-dns-over-https" title="Mozilla Firefox" target="_blank" rel="nofollow noopener noreferrer">Mozilla Firefox</a> supports <code class="language-text">DNS-over-HTTPS</code>.</li>
				</ul>
							<p>You will find more implementations <a href="https://dnscrypt.info/implementations" title="here" target="_blank" rel="nofollow noopener noreferrer">here</a> and <a href="https://dnsprivacy.org/wiki/display/DP/DNS+Privacy+Clients" title="here" target="_blank" rel="nofollow noopener noreferrer">here</a>.</p>

			<h3 id="support"><a href="#support" aria-hidden="true"><span class="icon icon-link"></span></a><u>Support</u></h3>
				<ul>
					<li><a href="https://ko-fi.com/arapurayil" title="Ko-fi" target="_blank" rel="nofollow noopener noreferrer">Ko-fi</a></li>
					<li><a href="https://liberapay.com/arapurayil" title="Liberapay" target="_blank" rel="nofollow noopener noreferrer">Liberapay</a></li>
				</ul>
		
		<h5><u>DISCLAIMER</u></h5>
		<p>Use at your own risk. Under no circumstances will the operator be held responsible or liable in any way for any claims, damages, losses, expenses, costs or liabilities whatsoever (including, without limitation, any direct or indirect damages for loss of profits, business interruption or loss of information) resulting or arising directly or indirectly from accessing or otherwise using this service.
		The operator does not guarantee in any way the access, availability and continuity of the functioning of this service. By using this website and service you consent to the disclaimer and agree to its terms and conditions.</p>
		<h5><u>PRIVACY POLICY</u></h5>
			<ul>
				<li>We do not (and will never) sell, license, sub-license or share any of the data submitted directly or indirectly by our users with any person or entity.</li>
				<li>When the service comes into contact with user data that shall not be logged, it is discarded as quickly as possible.</li>
				<li>We protect our users from privacy exposure to other services that we must interact with in order to operate properly.</li>
			</ul>
	</div>
  </Layout>
</template>

<static-query>
query {
  metadata {
    siteName
  }
}
</static-query>

<script>
import GitLink from '~/components/GitLink.vue'
import Shortcut from '~/components/Shortcut.vue'

export default {
  components: {
    GitLink,
    Shortcut
  },
  data() {
    return {
      description: 'Encrypted ad-blocking DNS resolver located in Mumbai, India'
    }
  },
  metaInfo() {
    return {
      title: this.description,
      meta: [
        { key: 'description', name: 'description', content: 'Encrypted ad-blocking DNS resolver located in Mumbai, India' }
      ]
    }
  }
}
</script>

<style lang="scss" scoped>
.content {
  display: flex;
  flex-direction: column;
}
.conf {
  display: flex;
   overflow: auto;
  flex-direction: column;
}

h1 {
  text-align: center;
  max-width: 600px;
  margin: 1.5em auto 1.5em;

  @include respond-above(md) {
    max-width: 1000px;
  }
}

h2 {
  font-size: 1.4rem;
  margin: 0;
}

nav {
  display: flex;
  justify-content: space-between;
  flex-direction: column;

  @include respond-above(sm) {
    flex-direction: row;
  }
}

.git {
  margin: 3em 0 0;
  align-self: center;

  @include respond-above(md) {
    margin: 5em 0 0;
  }
}
</style>
