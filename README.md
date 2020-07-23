# go-sdk
Golang SDK for communicating with Lyrid Platform

The SDK works under a singleton that manages Lyrid token and sessions internally. To download and use in your project:
<code>
go get github.com/LyridInc/go-sdk
</code>

Then import in your project:

<code>
import "github.com/LyridInc/go-sdk"
</code>

Initialization:
<br />
You can initialize the SDK by calling:

<code> 
sdk.GetInstance().Initialize(key, secret)
</code>

Where key and secret is the credentials from Lyrid. You can also use the SDK without initialization by setting LYRID_ACCESS and LYRID_SECRET as your environment variables.

Usage:

<code>
sdk.GetInstance().GetUserProfile()
sdk.GetInstance().GetAccountProfile()
</code>