---
-api-id: T:Windows.Media.Core.MediaStreamSourceStartingRequestDeferral
-api-type: winrt class
---

<!-- Class syntax.
public class MediaStreamSourceStartingRequestDeferral : Windows.Media.Core.IMediaStreamSourceStartingRequestDeferral
-->

# Windows.Media.Core.MediaStreamSourceStartingRequestDeferral

## -description
Provides a way for the application to asynchronously report that it has completed processing the [MediaStreamSource.Starting](mediastreamsource_starting.md) event.

## -remarks
You can use a deferral when you want to make an asynchronous call in response to the [MediaStreamSource.Starting](mediastreamsource_starting.md) event. For example, if you need to establish a HTTP connection or open a file for reading. The [MediaStreamSource](mediastreamsource.md) will then wait for you to mark the deferral as complete before it begins raising the [SampleRequested](mediastreamsource_samplerequested.md) event.

To create a deferral, call the [GetDeferral](mediastreamsourcestartingrequest_getdeferral.md) method on the [MediaStreamSourceStartingRequest](mediastreamsourcestartingrequest.md) object to instruct the [MediaStreamSource](mediastreamsource.md) to wait for your asynchronous call to complete. When you are ready to start receiving [SampleRequested](mediastreamsource_samplerequested.md) events, call the [Complete](mediastreamsourcestartingrequestdeferral_complete.md) method to end the deferral.

See the [MediaStreamSource Sample](http://go.microsoft.com/fwlink/p/?LinkID=309021) for an example of using Media Stream Source in a UWP app.

## -examples

## -see-also
[MediaStreamSource Sample](http://go.microsoft.com/fwlink/p/?LinkID=309021)