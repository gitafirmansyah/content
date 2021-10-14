---
title: Event reference
slug: Web/Events
tags:
  - Event
  - Overview
  - Reference
---
<p><a href="/en-US/docs/Learn/JavaScript/Building_blocks/Events">Events</a> are fired to notify code of "interesting changes" that may affect code execution. These can arise from user interactions such as using a mouse or resizing a window, changes in the state of the underlying environment (e.g. low battery or media events from the operating system), and other causes.</p>

<p>Each event is represented by an object that is based on the {{domxref("Event")}} interface, and may have additional custom fields and/or functions to provide information about what happened. The documentation for every event has a table (near the top) that includes a link to the associated event interface, and other relevant information. A full list of the different event types is given in <a href="/en-US/docs/Web/API/Event#introduction">Event > Interfaces based on Event</a>.</p>

<p><span class="seoSummary">This topic provides an index to the main <em>sorts</em> of events you might be interested in (animation, clipboard, workers etc.) along with the main classes that implement those sorts of events. At the end is a flat list of all documented events.</span></p>

<div class="notecard note">
	<p><strong>Note:</strong> This page lists many of the most common events you'll come across on the web. If you are searching for an event that isn't listed here, try searching for its name, topic area, or associated specification on the rest of MDN.</p>
</div>

<h2 id="Event_index">Event index</h2>

<table class="standard-table">
	<tr>
		<th>Event type</th>
		<th style="width: 50%">Description</th>
		<th>Documentation</th>
	</tr>

  <tr>
		<td>Animation</td>
		<td>
			<p>Events related to the <a href="/en-US/docs/Web/API/Web_Animations_API">Web Animation API</a>.</p>
			<p>Used to respond to changes in animation status (e.g. when an animation starts or ends).</p>
		</td>
		<td>Animation events fired on <a href="/en-US/docs/Web/API/Document#animation_events"><code>Document</code></a>, <a href="/en-US/docs/Web/API/Window#animation_events"><code>Window</code></a>, <a href="/en-US/docs/Web/API/HTMLElement#animation_events"><code>HTMLElement</code></a>.</td>
	</tr>

  <tr>
		<td>Asynchronous data fetching</td>
		<td>
			<p>Events related to the fetching data.</p>
		</td>
		<td>Events fired on <a href="/en-US/docs/Web/API/AbortSignal#events"><code>AbortSignal</code></a>, <a href="/en-US/docs/Web/API/XMLHttpRequest#events"><code>XMLHttpRequest</code></a>, <a href="/en-US/docs/Web/API/FileReader#events"><code>FileReader</code></a>.</td>
	</tr>


	<tr>
		<td>Clipboard</td>
		<td>
			<p>Events related to the <a href="/en-US/docs/Web/API/Clipboard_API">Clipboard API</a>.</p>
			<p>Used to notify when content is cut, copied, or pasted.</p>
		</td>
		<td>Events fired on <a href="/en-US/docs/Web/API/Document#clipboard_events"><code>Document</code></a>, <a href="/en-US/docs/Web/API/Element#clipboard_events"><code>Element</code></a>, <a href="/en-US/docs/Web/API/Window#clipboard_events"><code>Window</code></a>.
		</td>
	</tr>

	<tr>
		<td>Composition</td>
		<td>
			<p>Events related to composition; entering text "indirectly" (rather than using normal keyboard presses).</p>
			<p>For example, text entered via a speech to text engine, or using special key combinations that modify keyboard presses to represent new characters in another language.</p>
		</td>
		<td>Events fired on <a href="/en-US/docs/Web/API/Element#composition_events"><code>Element</code></a>.
		</td>
	</tr>

	<tr>
		<td>CSS transition</td>
		<td>
			<p>Events related to <a href="/en-US/docs/Web/CSS/CSS_Transitions">CSS Transitions</a>.</p>
			<p>Provides notification events when CSS transitions start, stop, are cancelled, etc.</p>
		</td>
		<td>Events fired on <a href="/en-US/docs/Web/API/Document#transition_events"><code>Document</code></a>, <a href="/en-US/docs/Web/API/HTMLElement#transition_events"><code>HTMLElement</code></a>, <a href="/en-US/docs/Web/API/Window#transition_events"><code>Window</code></a>.</td>
	</tr>

	<tr>
		<td>Database</td>
		<td>
			<p>Events related to database operations: opening, closing, transactions, errors, etc.</p>
		</td>
		<td>Events fired on <a href="/en-US/docs/Web/API/IDBDatabase#events"><code>IDBDatabase</code></a>, <a href="/en-US/docs/Web/API/IDBOpenDBRequest#events"><code>IDBOpenDBRequest</code></a>, <a href="/en-US/docs/Web/API/IDBRequest#events"><code>IDBRequest</code></a>, <a href="/en-US/docs/Web/API/IDBTransaction#events"><code>IDBTransaction</code></a>.</td>
	</tr>

  <tr>
		<td>DOM mutation</td>
		<td>
			<p>Events related to modifications to the Document Object Model (DOM) hierarchy and nodes.</p>
		</td>
		<td>
      <div class="notecard warning">
        <p><strong>Warning:</strong> <a href="/en-US/docs/Web/API/MutationEvent">Mutation Events</a> are deprecated. <a href="/en-US/docs/Web/API/MutationObserver">Mutation Observers</a> should be used instead.</p>
      </div>
    </td>
	</tr>

	<tr>
		<td>Drag'n'drop, Wheel</td>
		<td>
			<p>Events related to using the <a href="/en-US/docs/Web/API/HTML_Drag_and_Drop_API">HTML Drag and Drop API</a> and <a href="/en-US/docs/Web/API/WheelEvent">wheel events</a>.</p>
			<p>Drag and Wheel events are derived from mouse events. While they are fired when using mouse wheel or drag/drop, they may also be used with other appropriate hardware.</p>
		</td>
		<td>
			<p>Drag events fired on <a href="/en-US/docs/Web/API/Document#drag_drop_events"><code>Document</code></a></p>
			<p>Wheel events fired on <a href="/en-US/docs/Web/API/Document/wheel_event"><code>Document</code></a> and <a href="/en-US/docs/Web/API/Element/wheel_event"><code>Element</code></a></p>
		</td>
	</tr>

	<tr>
		<td>Focus</td>
		<td>
			<p>Events related to elements gaining and losing focus.</p>
		</td>
		<td>Events fired on <a href="/en-US/docs/Web/API/Element#focus_events"><code>Element</code></a>, <a href="/en-US/docs/Web/API/Window#focus_events"><code>Window</code></a>.
		</td>
	</tr>

	<tr>
		<td>Form</td>
		<td>
			<p>Events related to forms being constructed, reset and submitted.</p>
		</td>
		<td>Events fired on <a href="/en-US/docs/Web/API/HTMLFormElement#events"><code>HTMLFormElement</code></a>.
		</td>
	</tr>


	<tr>
		<td>Fullscreen</td>
		<td>
			<p>Events related to the <a href="/en-US/docs/Web/API/Fullscreen_API">Fullscreen API</a>.</p>
			<p>Used to notify when the transitioning between full screen and windowed modes, and also of errors occurring during this transition.</p>
		</td>
		<td>Events fired on <a href="/en-US/docs/Web/API/Document#fullscreen_events"><code>Document</code></a>, <a href="/en-US/docs/Web/API/Element#fullscreen_events"><code>Element</code></a>.</td>
	</tr>


	<tr>
		<td>Gamepad</td>
		<td>
			<p>Events related to the <a href="/en-US/docs/Web/API/Gamepad_API">Gamepad API</a>.</p>
		</td>
		<td>Events fired on <a href="/en-US/docs/Web/API/Window#gamepad_events"><code>Window</code></a>.
		</td>
	</tr>

  <tr>
		<td>Gestures</td>
		<td>
      <p><a href="/en-US/docs/Web/API/Touch_events">Touch events</a> are recommended for implementing gestures.</p>
		</td>
		<td>
      <p>Events fired on <a href="/en-US/docs/Web/API/Document#touch_events"><code>Document</code></a>, <a href="/en-US/docs/Web/API/Element#touch_events"><code>Element</code></a>.</p>
      <p>In addition there are a number of non-standard gesture events:</p>
      <ul>
        <li>Non-standard WebKit specific events on <a href="/en-US/docs/Web/API/Element#touch_events"><code>Element</code></a>: <a href="/en-US/docs/Web/API/Element/gesturestart_event"><code>gesturestart</code> event</a>, <a href="/en-US/docs/Web/API/Element/gesturechange_event"><code>gesturechange</code> event</a>, <a href="/en-US/docs/Web/API/Element/gestureend_event"><code>gestureend</code> event</a>.
        </li>
        <li>Non-standard IE specific events on <a href="/en-US/docs/Web/API/Element#touch_events"><code>Element</code></a>: <a href="/en-US/docs/Web/API/Element/MSGestureStart_event"><code>MSGestureStart</code></a>, <a href="/en-US/docs/Web/API/Element/MSGestureChange_event"><code>MSGestureChange</code></a>, <a href="/en-US/docs/Web/API/Element/MSGestureEnd_event"><code>MSGestureEnd</code></a>, <a href="/en-US/docs/Web/API/Element/MSGestureHold_event"><code>MSGestureHold</code></a>, <a href="/en-US/docs/Web/API/Element/MSGestureTap_event"><code>MSGestureTap</code></a>.</li>
        <li>Deprecated/non-standard Mozilla touch events <a href="/en-US/docs/Web/API/Touch_events/Mozilla_experimental_events">Touch events (Mozilla experimental)</a></li>
        <li><a href="/en-US/docs/Web/Events/Mouse_gesture_events">Mouse gesture events for Firefox Addons</a></li>
      </ul>
		</td>
	</tr>

	<tr>
		<td>History</td>
		<td>
			<p>Events related to the <a href="/en-US/docs/Web/API/History_API">History API</a>.</p>
		</td>
		<td>Events fired on <a href="/en-US/docs/Web/API/Window#history_events"><code>Window</code></a>.
		</td>
	</tr>

  <tr>
		<td>HTML element content display management</td>
		<td>
			<p>Events related to changing the state of a display or textual element.</p>
		</td>
		<td>Events fired on <a href="/en-US/docs/Web/API/HTMLDetailsElement#events"><code>HTMLDetailsElement</code></a>, <a href="/en-US/docs/Web/API/HTMLDialogElement#events"><code>HTMLDialogElement</code></a>, <a href="/en-US/docs/Web/API/HTMLSlotElement#events"><code>HTMLSlotElement</code></a>.
		</td>
	</tr>

	<tr>
		<td>Inputs</td>
		<td>
			<p>Events related to HTML input elements e.g. {{HTMLElement("input")}}, {{HTMLElement("select")}}, or {{HTMLElement("textarea")}}.</p>
		</td>
		<td>Events fired on <a href="/en-US/docs/Web/API/HTMLElement#input_events"><code>HTMLElement</code></a>, <a href="/en-US/docs/Web/API/HTMLInputElement#events"><code>HTMLInputElement</code></a>.</td>
	</tr>

	<tr>
		<td>Keyboard</td>
		<td>
			<p>Events related to using a <a href="/en-US/docs/Web/API/KeyboardEvent">keyboard</a>.</p>
			<p>Used to notify when keys are moved up, down, or just pressed.</p>
		</td>
		<td>Events fired on <a href="/en-US/docs/Web/API/Document#keyboard_events"><code>Document</code></a>, <a href="/en-US/docs/Web/API/Element#keyboard_events"><code>Element</code></a>.
		</td>
	</tr>

	<tr>
		<td>Loading/unloading documents</td>
		<td>
			<p>Events related to loading and unloading documents.</p>
		</td>
		<td>
			<p>Events fired on <a href="/en-US/docs/Web/API/Document#load_unload_events"><code>Document</code></a> and <a href="/en-US/docs/Web/API/Window#load_unload_events"><code>Window</code></a>.</p>
		</td>
	</tr>

	<tr>
		<td>Manifests</td>
		<td>
			<p>Events related to installation of <a href="/en-US/docs/Web/Manifest">progressive web app manifests</a>.</p>
		</td>
		<td>Events fired on <a href="/en-US/docs/Web/API/Window#manifest_events"><code>Window</code></a>.</td>
	</tr>

	<tr id="media">
		<td>Media</td>
		<td>
			<p>Events related to media usage (including the <a href="/en-US/docs/Web/API/Media_Streams_API#events">Media Capture and Streams API</a>, <a href="/en-US/docs/Web/API/Web_Audio_API#events">Web Audio API</a>, <a href="/en-US/docs/Web/API/Picture-in-Picture_API#events">Picture-in-Picture API</a>, etc.).</p>
		</td>
		<td>Events fired on <a href="/en-US/docs/Web/API/ScriptProcessorNode#events"><code>ScriptProcessorNode</code></a>, <a href="/en-US/docs/Web/API/HTMLMediaElement#events"><code>HTMLMediaElement</code></a>, <a href="/en-US/docs/Web/API/AudioTrackList#events"><code>AudioTrackList</code></a>, <a href="/en-US/docs/Web/API/AudioScheduledSourceNode#events"><code>AudioScheduledSourceNode</code></a>, <a href="/en-US/docs/Web/API/MediaRecorder#events"><code>MediaRecorder</code></a>, <a href="/en-US/docs/Web/API/MediaStream#events"><code>MediaStream</code></a>, <a href="/en-US/docs/Web/API/MediaStreamTrack"><code>MediaStreamTrack</code></a>, <a href="/en-US/docs/Web/API/VideoTrackList#events"><code>VideoTrackList</code></a>, <a href="/en-US/docs/Web/API/HTMLTrackElement#events"><code>HTMLTrackElement</code></a>, <a href="/en-US/docs/Web/API/OfflineAudioContext#events"><code>OfflineAudioContext</code></a>, <a href="/en-US/docs/Web/API/TextTrack#events"><code>TextTrack</code></a>, <a href="/en-US/docs/Web/API/TextTrackList#events"><code>TextTrackList</code></a>, <a href="/en-US/docs/Web/HTML/Element/audio#events">Element/audio</a>, <a href="/en-US/docs/Web/HTML/Element/video#events">Element/video</a>.
		</td>
	</tr>

	<tr>
		<td>Messaging</td>
		<td>
			<p>Events related to a window receiving a message from another browsing context.</p>
		</td>
		<td>Events fired on <a href="/en-US/docs/Web/API/Window#messaging_events"><code>Window</code></a>.</td>
	</tr>

	<tr>
		<td>Mouse</td>
		<td>
			<p>Events related to using a <a href="/en-US/docs/Web/API/MouseEvent">computer mouse</a>.</p>
			<p>Used to notify when the mouse is clicked, doubleclicked, up and down events, right-click, movement in and out of an element, text selection, etc.</p>
			<p>Pointer events provide a hardware-agnostic alternative to mouse events. Drag and Wheel events are derived from mouse events.</p>
		</td>
		<td>Mouse events fired on <a href="/en-US/docs/Web/API/Element#mouse_events"><code>Element</code></a></td>
	</tr>

	<tr>
		<td>Network/Connection</td>
		<td>
			<p>Events related to gaining and losing network connection.</p>
		</td>
		<td>
			<p>Events fired on <a href="/en-US/docs/Web/API/Window#connection_events"><code>Window</code></a>.</p>
			<p>Events fired on <a href="/en-US/docs/Web/API/NetworkInformation#event_handler"><code>NetworkInformation</code></a> (<a href="/en-US/docs/Web/API/Network_Information_API">Network Information API</a>).</p>
		</td>
	</tr>

	<tr>
		<td>Payments</td>
		<td>
			<p>Events related to the <a href="/en-US/docs/Web/API/Payment_Request_API">Payment Request API</a>.</p>
		</td>
		<td>
			<p>Events fired on <a href="/en-US/docs/Web/API/PaymentRequest#events"><code>PaymentRequest</code></a>, <a href="/en-US/docs/Web/API/PaymentResponse#events"><code>PaymentResponse</code></a>.</p>
		</td>
	</tr>

	<tr>
		<td>Performance</td>
		<td>
			<p>Events related to <a href="/en-US/docs/Web/API/Performance_API">High Resolution Time API</a>, <a href="/en-US/docs/Web/API/Performance_Timeline">Performance Timeline API</a>, <a href="/en-US/docs/Web/API/Navigation_timing_API">Navigation Timing API</a>, <a href="/en-US/docs/Web/API/User_Timing_API">User Timing API</a>, and <a href="/en-US/docs/Web/API/Resource_Timing_API">Resource Timing API</a>.</p>
		</td>
		<td>
			<p>Events fired on <a href="/en-US/docs/Web/API/Performance#events"><code>Performance</code></a>.</p>
		</td>
	</tr>

	<tr>
		<td>Pointer</td>
		<td>
			<p>Events related to the <a href="/en-US/docs/Web/API/Pointer_events">Pointer Events API</a>.</p>
			<p>Provides hardware-agnostic notification from pointing devices including Mouse, Touch, pen/stylus.</p>
		</td>
		<td>Events fired on <a href="/en-US/docs/Web/API/Document#pointer_events"><code>Document</code></a>, <a href="/en-US/docs/Web/API/HTMLElement#pointer_events"><code>HTMLElement</code></a>.</td>
	</tr>

	<tr>
		<td>Print</td>
		<td>
			<p>Events related to printing.</p>
		</td>
		<td>Events fired on <a href="/en-US/docs/Web/API/Window#print_events"><code>Window</code></a>.</td>
	</tr>

	<tr>
		<td>Promise rejection</td>
		<td>
			<p>Events sent to the global script context when any JavaScript promise is rejected.</p>
		</td>
		<td>Events fired on <a href="/en-US/docs/Web/API/Window#promise_rejection_events"><code>Window</code></a>.</td>
	</tr>

	<tr>
		<td>Sockets</td>
		<td>
			<p>Events related to the <a href="/en-US/docs/Web/API/WebSockets_API">WebSockets API</a>.</p>
		</td>
		<td>Events fired on <a href="/en-US/docs/Web/API/WebSocket#events"><code>Websocket</code></a>.</td>
	</tr>



	<tr>
		<td>SVG</td>
		<td>
			<p>Events related to SVG images.</p>
		</td>
		<td>
			<p>Events fired on <a href="/en-US/docs/Web/API/SVGElement#events"><code>SVGElement</code></a>, <a href="/en-US/docs/Web/API/SVGAnimationElement#events"><code>SVGAnimationElement</code></a>, <a href="/en-US/docs/Web/API/SVGGraphicsElement#events"><code>SVGGraphicsElement</code></a>.</p>
		</td>
	</tr>

	<tr>
		<td>Text selection</td>
		<td>
			<p><a href="/en-US/docs/Web/API/Selection">Selection API</a> events related to selecting text.</p>
		</td>
		<td>
			<p>Event (<code>selectionchange</code>) fired on {{domxref("HTMLTextAreaElement/selectionchange_event", "HTMLTextAreaElement")}}, {{domxref("HTMLInputElement/selectionchange_event", "HTMLInputElement")}}.</p>
		</td>
	</tr>

	<tr>
		<td>Touch</td>
		<td>
			<p>Events related to the <a href="/en-US/docs/Web/API/Touch_events">Touch Events API</a>.</p>
			<p>Provides notification events from interacting with a touch sensitive screen (i.e. using a finger or stylus). Not related to the <a href="/en-US/docs/Web/API/Force_Touch_events#events">Force Touch API</a>.</p>
		</td>
		<td>Events fired on <a href="/en-US/docs/Web/API/Document#touch_events"><code>Document</code></a>, <a href="/en-US/docs/Web/API/Element#touch_events"><code>Element</code></a>.</td>
	</tr>

	<tr>
		<td>Virtual reality</td>
		<td>
			<p>Events related to the <a href="/en-US/docs/Web/API/WebXR_Device_API">WebXR Device API</a>.</p>
			<div class="notecard warning">
				<p><strong>Warning:</strong> The <a href="/en-US/docs/Web/API/WebVR_API">WebVR API</a> (and associated <a href="/en-US/docs/Web/API/Window#webvr_events"><code>Window</code> events</a>) are deprecated.</p>
			</div>
		</td>
		<td>Events fired on <a href="/en-US/docs/Web/API/XRSystem#events"><code>XRSystem</code></a>, <a href="/en-US/docs/Web/API/XRSession#events"><code>XRSession</code></a>, <a href="/en-US/docs/Web/API/XRReferenceSpace#events"><code>XRReferenceSpace</code></a>.</td>
	</tr>

	<tr>
		<td>RTC (real time communication)</td>
		<td>
			<p>Events related to the <a href="/en-US/docs/Web/API/WebRTC_API">WebRTC API</a>.</p>
		</td>
		<td>Events fired on <a href="/en-US/docs/Web/API/RTCDataChannel#events"><code>RTCDataChannel</code></a>, <a href="/en-US/docs/Web/API/RTCDTMFSender#events"><code>RTCDTMFSender</code></a>, <a href="/en-US/docs/Web/API/RTCIceTransport#events"><code>RTCIceTransport</code></a>, <a href="/en-US/docs/Web/API/RTCPeerConnection#events"><code>RTCPeerConnection</code></a>.</td>
	</tr>

  <tr>
		<td>Server-sent events</td>
		<td>
			<p>Events related to the <a href="/en-US/docs/Web/API/Server-sent_events">server sent events API</a>.</p>
		</td>
		<td>Events fired on <a href="/en-US/docs/Web/API/EventSource#events"><code>EventSource</code></a>.
		</td>
	</tr>

	<tr>
		<td>Speech</td>
		<td>
			<p>Events related to the <a href="/en-US/docs/Web/API/Web_Speech_API">Web Speech API</a>.</p>
		</td>
		<td>Events fired on <a href="/en-US/docs/Web/API/SpeechSynthesisUtterance#events"><code>SpeechSynthesisUtterance</code></a>.</td>
	</tr>

	<tr>
		<td>Workers</td>
		<td>
			<p>Events related to the <a href="/en-US/docs/Web/API/Web_Workers_API">Web Workers API</a>, <a href="/en-US/docs/Web/API/Service_Worker_API">Service Worker API</a>, <a href="/en-US/docs/Web/API/Broadcast_Channel_API">Broadcast Channel API</a>, and <a href="/en-US/docs/Web/API/Channel_Messaging_API">Channel Messaging API</a>.</p>
			<p>Used to respond to new messages and message sending errors. Service workers can also be notified of other events, including push notifications, users clicking on displayed notifications, that push subscription has been invalidated, deletion of items from the content index, etc.</p>
		</td>
		<td>Events fired on <a href="/en-US/docs/Web/API/ServiceWorkerGlobalScope#events"><code>ServiceWorkerGlobalScope</code></a>, <a href="/en-US/docs/Web/API/DedicatedWorkerGlobalScope#events"><code>DedicatedWorkerGlobalScope</code></a>, <a href="/en-US/docs/Web/API/SharedWorkerGlobalScope#events"><code>SharedWorkerGlobalScope</code></a>, <a href="/en-US/docs/Web/API/WorkerGlobalScope#events"><code>WorkerGlobalScope</code></a>, <a href="/en-US/docs/Web/API/Worker#events"><code>Worker</code></a>, <a href="/en-US/docs/Web/API/WorkerGlobalScope#events"><code>WorkerGlobalScope</code></a>, <a href="/en-US/docs/Web/API/BroadcastChannel#events"><code>BroadcastChannel</code></a>, <a href="/en-US/docs/Web/API/MessagePort#events"><code>MessagePort</code></a>.
		</td>
	</tr>

</table>


<h2>Event listing</h2>

<p>This section lists events that have <em>their own</em> reference pages on MDN. If you are interested in an event that isn't listed here, try searching for its name, topic area, or associated specification on the rest of MDN.</p>

<ul>
  <li>{{DOMxRef("AbortSignal")}}
    <ul>
      <li><a href="/en-US/docs/Web/API/AbortSignal/abort_event">abort event</a></li>
    </ul>
  </li>
  <li>{{DOMxRef("AudioScheduledSourceNode")}}
    <ul>
      <li><a href="/en-US/docs/Web/API/AudioScheduledSourceNode/ended_event">ended event</a></li>
    </ul>
  </li>
  <li>{{DOMxRef("AudioTrackList")}}
    <ul>
      <li><a href="/en-US/docs/Web/API/AudioTrackList/addtrack_event">addtrack event</a></li>
      <li><a href="/en-US/docs/Web/API/AudioTrackList/change_event">change event</a></li>
      <li><a href="/en-US/docs/Web/API/AudioTrackList/removetrack_event">removetrack event</a></li>
    </ul>
  </li>
  <li>{{DOMxRef("BroadcastChannel")}}
    <ul>
      <li><a href="/en-US/docs/Web/API/BroadcastChannel/messageerror_event">messageerror event</a></li>
      <li><a href="/en-US/docs/Web/API/BroadcastChannel/message_event">message event</a></li>
    </ul>
  </li>
  <li>{{DOMxRef("DedicatedWorkerGlobalScope")}}
    <ul>
      <li><a href="/en-US/docs/Web/API/DedicatedWorkerGlobalScope/messageerror_event">messageerror event</a></li>
      <li><a href="/en-US/docs/Web/API/DedicatedWorkerGlobalScope/message_event">message event</a></li>
    </ul>
  </li>
  <li>{{DOMxRef("Document")}}
    <ul>
      <li><a href="/en-US/docs/Web/API/Document/animationcancel_event">animationcancel event</a></li>
      <li><a href="/en-US/docs/Web/API/Document/animationend_event">animationend event</a></li>
      <li><a href="/en-US/docs/Web/API/Document/animationiteration_event">animationiteration event</a></li>
      <li><a href="/en-US/docs/Web/API/Document/animationstart_event">animationstart event</a></li>
      <li><a href="/en-US/docs/Web/API/Document/copy_event">copy event</a></li>
      <li><a href="/en-US/docs/Web/API/Document/cut_event">cut event</a></li>
      <li><a href="/en-US/docs/Web/API/Document/DOMContentLoaded_event">DOMContentLoaded event</a></li>
      <li><a href="/en-US/docs/Web/API/Document/dragend_event">dragend event</a></li>
      <li><a href="/en-US/docs/Web/API/Document/dragenter_event">dragenter event</a></li>
      <li><a href="/en-US/docs/Web/API/Document/dragleave_event">dragleave event</a></li>
      <li><a href="/en-US/docs/Web/API/Document/dragover_event">dragover event</a></li>
      <li><a href="/en-US/docs/Web/API/Document/dragstart_event">dragstart event</a></li>
      <li><a href="/en-US/docs/Web/API/Document/drag_event">drag event</a></li>
      <li><a href="/en-US/docs/Web/API/Document/drop_event">drop event</a></li>
      <li><a href="/en-US/docs/Web/API/Document/fullscreenchange_event">fullscreenchange event</a></li>
      <li><a href="/en-US/docs/Web/API/Document/fullscreenerror_event">fullscreenerror event</a></li>
      <li><a href="/en-US/docs/Web/API/Document/gotpointercapture_event">gotpointercapture event</a></li>
      <li><a href="/en-US/docs/Web/API/Document/keydown_event">keydown event</a></li>
      <li><a href="/en-US/docs/Web/API/Document/keypress_event">keypress event</a></li>
      <li><a href="/en-US/docs/Web/API/Document/keyup_event">keyup event</a></li>
      <li><a href="/en-US/docs/Web/API/Document/lostpointercapture_event">lostpointercapture event</a></li>
      <li><a href="/en-US/docs/Web/API/Document/paste_event">paste event</a></li>
      <li><a href="/en-US/docs/Web/API/Document/pointercancel_event">pointercancel event</a></li>
      <li><a href="/en-US/docs/Web/API/Document/pointerdown_event">pointerdown event</a></li>
      <li><a href="/en-US/docs/Web/API/Document/pointerenter_event">pointerenter event</a></li>
      <li><a href="/en-US/docs/Web/API/Document/pointerleave_event">pointerleave event</a></li>
      <li><a href="/en-US/docs/Web/API/Document/pointerlockchange_event">pointerlockchange event</a></li>
      <li><a href="/en-US/docs/Web/API/Document/pointerlockerror_event">pointerlockerror event</a></li>
      <li><a href="/en-US/docs/Web/API/Document/pointermove_event">pointermove event</a></li>
      <li><a href="/en-US/docs/Web/API/Document/pointerout_event">pointerout event</a></li>
      <li><a href="/en-US/docs/Web/API/Document/pointerover_event">pointerover event</a></li>
      <li><a href="/en-US/docs/Web/API/Document/pointerup_event">pointerup event</a></li>
      <li><a href="/en-US/docs/Web/API/Document/readystatechange_event">readystatechange event</a></li>
      <li><a href="/en-US/docs/Web/API/Document/scroll_event">scroll event</a></li>
      <li><a href="/en-US/docs/Web/API/Document/selectionchange_event">selectionchange event</a></li>
      <li><a href="/en-US/docs/Web/API/Document/selectstart_event">selectstart event</a></li>
      <li><a href="/en-US/docs/Web/API/Document/touchcancel_event">touchcancel event</a></li>
      <li><a href="/en-US/docs/Web/API/Document/touchend_event">touchend event</a></li>
      <li><a href="/en-US/docs/Web/API/Document/touchmove_event">touchmove event</a></li>
      <li><a href="/en-US/docs/Web/API/Document/touchstart_event">touchstart event</a></li>
      <li><a href="/en-US/docs/Web/API/Document/transitioncancel_event">transitioncancel event</a></li>
      <li><a href="/en-US/docs/Web/API/Document/transitionend_event">transitionend event</a></li>
      <li><a href="/en-US/docs/Web/API/Document/transitionrun_event">transitionrun event</a></li>
      <li><a href="/en-US/docs/Web/API/Document/transitionstart_event">transitionstart event</a></li>
      <li><a href="/en-US/docs/Web/API/Document/visibilitychange_event">visibilitychange event</a></li>
      <li><a href="/en-US/docs/Web/API/Document/wheel_event">wheel event</a></li>
    </ul>
  </li>
  <li>{{DOMxRef("Element")}}
    <ul>
      <li><a href="/en-US/docs/Web/API/Element/afterscriptexecute_event">afterscriptexecute event</a></li>
      <li><a href="/en-US/docs/Web/API/Element/auxclick_event">auxclick event</a></li>
      <li><a href="/en-US/docs/Web/API/Element/beforescriptexecute_event">beforescriptexecute event</a></li>
      <li><a href="/en-US/docs/Web/API/Element/blur_event">blur event</a></li>
      <li><a href="/en-US/docs/Web/API/Element/click_event">click event</a></li>
      <li><a href="/en-US/docs/Web/API/Element/compositionend_event">compositionend event</a></li>
      <li><a href="/en-US/docs/Web/API/Element/compositionstart_event">compositionstart event</a></li>
      <li><a href="/en-US/docs/Web/API/Element/compositionupdate_event">compositionupdate event</a></li>
      <li><a href="/en-US/docs/Web/API/Element/contextmenu_event">contextmenu event</a></li>
      <li><a href="/en-US/docs/Web/API/Element/copy_event">copy event</a></li>
      <li><a href="/en-US/docs/Web/API/Element/cut_event">cut event</a></li>
      <li><a href="/en-US/docs/Web/API/Element/dblclick_event">dblclick event</a></li>
      <li><a href="/en-US/docs/Web/API/Element/DOMActivate_event">DOMActivate event</a></li>
      <li><a href="/en-US/docs/Web/API/Element/DOMMouseScroll_event">DOMMouseScroll event</a></li>
      <li><a href="/en-US/docs/Web/API/Element/error_event">error event</a></li>
      <li><a href="/en-US/docs/Web/API/Element/focusin_event">focusin event</a></li>
      <li><a href="/en-US/docs/Web/API/Element/focusout_event">focusout event</a></li>
      <li><a href="/en-US/docs/Web/API/Element/focus_event">focus event</a></li>
      <li><a href="/en-US/docs/Web/API/Element/fullscreenchange_event">fullscreenchange event</a></li>
      <li><a href="/en-US/docs/Web/API/Element/fullscreenerror_event">fullscreenerror event</a></li>
      <li><a href="/en-US/docs/Web/API/Element/gesturechange_event">gesturechange event</a></li>
      <li><a href="/en-US/docs/Web/API/Element/gestureend_event">gestureend event</a></li>
      <li><a href="/en-US/docs/Web/API/Element/gesturestart_event">gesturestart event</a></li>
      <li><a href="/en-US/docs/Web/API/Element/keydown_event">keydown event</a></li>
      <li><a href="/en-US/docs/Web/API/Element/keypress_event">keypress event</a></li>
      <li><a href="/en-US/docs/Web/API/Element/keyup_event">keyup event</a></li>
      <li><a href="/en-US/docs/Web/API/Element/mousedown_event">mousedown event</a></li>
      <li><a href="/en-US/docs/Web/API/Element/mouseenter_event">mouseenter event</a></li>
      <li><a href="/en-US/docs/Web/API/Element/mouseleave_event">mouseleave event</a></li>
      <li><a href="/en-US/docs/Web/API/Element/mousemove_event">mousemove event</a></li>
      <li><a href="/en-US/docs/Web/API/Element/mouseout_event">mouseout event</a></li>
      <li><a href="/en-US/docs/Web/API/Element/mouseover_event">mouseover event</a></li>
      <li><a href="/en-US/docs/Web/API/Element/mouseup_event">mouseup event</a></li>
      <li><a href="/en-US/docs/Web/API/Element/mousewheel_event">mousewheel event</a></li>
      <li><a href="/en-US/docs/Web/API/Element/msContentZoom_event">msContentZoom event</a></li>
      <li><a href="/en-US/docs/Web/API/Element/MSGestureChange_event">MSGestureChange event</a></li>
      <li><a href="/en-US/docs/Web/API/Element/MSGestureEnd_event">MSGestureEnd event</a></li>
      <li><a href="/en-US/docs/Web/API/Element/MSGestureHold_event">MSGestureHold event</a></li>
      <li><a href="/en-US/docs/Web/API/Element/MSGestureStart_event">MSGestureStart event</a></li>
      <li><a href="/en-US/docs/Web/API/Element/MSGestureTap_event">MSGestureTap event</a></li>
      <li><a href="/en-US/docs/Web/API/Element/MSInertiaStart_event">MSInertiaStart event</a></li>
      <li><a href="/en-US/docs/Web/API/Element/MSManipulationStateChanged_event">MSManipulationStateChanged event</a></li>
      <li><a href="/en-US/docs/Web/API/Element/overflow_event">overflow event</a></li>
      <li><a href="/en-US/docs/Web/API/Element/paste_event">paste event</a></li>
      <li><a href="/en-US/docs/Web/API/Element/scroll_event">scroll event</a></li>
      <li><a href="/en-US/docs/Web/API/Element/select_event">select event</a></li>
      <li><a href="/en-US/docs/Web/API/Element/show_event">show event</a></li>
      <li><a href="/en-US/docs/Web/API/Element/touchcancel_event">touchcancel event</a></li>
      <li><a href="/en-US/docs/Web/API/Element/touchend_event">touchend event</a></li>
      <li><a href="/en-US/docs/Web/API/Element/touchmove_event">touchmove event</a></li>
      <li><a href="/en-US/docs/Web/API/Element/touchstart_event">touchstart event</a></li>
      <li><a href="/en-US/docs/Web/API/Element/underflow_event">underflow event</a></li>
      <li><a href="/en-US/docs/Web/API/Element/webkitmouseforcechanged_event">webkitmouseforcechanged event</a></li>
      <li><a href="/en-US/docs/Web/API/Element/webkitmouseforcedown_event">webkitmouseforcedown event</a></li>
      <li><a href="/en-US/docs/Web/API/Element/webkitmouseforceup_event">webkitmouseforceup event</a></li>
      <li><a href="/en-US/docs/Web/API/Element/webkitmouseforcewillbegin_event">webkitmouseforcewillbegin event</a></li>
      <li><a href="/en-US/docs/Web/API/Element/wheel_event">wheel event</a></li>
    </ul>
  </li>
  <li>{{DOMxRef("EventSource")}}
    <ul>
      <li><a href="/en-US/docs/Web/API/EventSource/error_event">error event</a></li>
      <li><a href="/en-US/docs/Web/API/EventSource/message_event">message event</a></li>
      <li><a href="/en-US/docs/Web/API/EventSource/open_event">open event</a></li>
    </ul>
  </li>
  <li>{{DOMxRef("FileReader")}}
    <ul>
      <li><a href="/en-US/docs/Web/API/FileReader/abort_event">abort event</a></li>
      <li><a href="/en-US/docs/Web/API/FileReader/error_event">error event</a></li>
      <li><a href="/en-US/docs/Web/API/FileReader/loadend_event">loadend event</a></li>
      <li><a href="/en-US/docs/Web/API/FileReader/loadstart_event">loadstart event</a></li>
      <li><a href="/en-US/docs/Web/API/FileReader/load_event">load event</a></li>
      <li><a href="/en-US/docs/Web/API/FileReader/progress_event">progress event</a></li>
    </ul>
  </li>
  <li>{{DOMxRef("HTMLCanvasElement")}}
    <ul>
      <li><a href="/en-US/docs/Web/API/HTMLCanvasElement/webglcontextcreationerror_event">webglcontextcreationerror event</a></li>
      <li><a href="/en-US/docs/Web/API/HTMLCanvasElement/webglcontextlost_event">webglcontextlost event</a></li>
      <li><a href="/en-US/docs/Web/API/HTMLCanvasElement/webglcontextrestored_event">webglcontextrestored event</a></li>
    </ul>
  </li>
  <li>{{DOMxRef("HTMLDetailsElement")}}
    <ul>
      <li><a href="/en-US/docs/Web/API/HTMLDetailsElement/toggle_event">toggle event</a></li>
    </ul>
  </li>
  <li>{{DOMxRef("HTMLDialogElement")}}
    <ul>
      <li><a href="/en-US/docs/Web/API/HTMLDialogElement/cancel_event">cancel event</a></li>
      <li><a href="/en-US/docs/Web/API/HTMLDialogElement/close_event">close event</a></li>
    </ul>
  </li>
  <li>{{DOMxRef("HTMLElement")}}
    <ul>
      <li><a href="/en-US/docs/Web/API/HTMLElement/animationcancel_event">animationcancel event</a></li>
      <li><a href="/en-US/docs/Web/API/HTMLElement/animationend_event">animationend event</a></li>
      <li><a href="/en-US/docs/Web/API/HTMLElement/animationiteration_event">animationiteration event</a></li>
      <li><a href="/en-US/docs/Web/API/HTMLElement/animationstart_event">animationstart event</a></li>
      <li><a href="/en-US/docs/Web/API/HTMLElement/beforeinput_event">beforeinput event</a></li>
      <li><a href="/en-US/docs/Web/API/HTMLElement/change_event">change event</a></li>
      <li><a href="/en-US/docs/Web/API/HTMLElement/gotpointercapture_event">gotpointercapture event</a></li>
      <li><a href="/en-US/docs/Web/API/HTMLElement/input_event">input event</a></li>
      <li><a href="/en-US/docs/Web/API/HTMLElement/lostpointercapture_event">lostpointercapture event</a></li>
      <li><a href="/en-US/docs/Web/API/HTMLElement/pointercancel_event">pointercancel event</a></li>
      <li><a href="/en-US/docs/Web/API/HTMLElement/pointerdown_event">pointerdown event</a></li>
      <li><a href="/en-US/docs/Web/API/HTMLElement/pointerenter_event">pointerenter event</a></li>
      <li><a href="/en-US/docs/Web/API/HTMLElement/pointerleave_event">pointerleave event</a></li>
      <li><a href="/en-US/docs/Web/API/HTMLElement/pointermove_event">pointermove event</a></li>
      <li><a href="/en-US/docs/Web/API/HTMLElement/pointerout_event">pointerout event</a></li>
      <li><a href="/en-US/docs/Web/API/HTMLElement/pointerover_event">pointerover event</a></li>
      <li><a href="/en-US/docs/Web/API/HTMLElement/pointerup_event">pointerup event</a></li>
      <li><a href="/en-US/docs/Web/API/HTMLElement/transitioncancel_event">transitioncancel event</a></li>
      <li><a href="/en-US/docs/Web/API/HTMLElement/transitionend_event">transitionend event</a></li>
      <li><a href="/en-US/docs/Web/API/HTMLElement/transitionrun_event">transitionrun event</a></li>
      <li><a href="/en-US/docs/Web/API/HTMLElement/transitionstart_event">transitionstart event</a></li>
    </ul>
  </li>
  <li>{{DOMxRef("HTMLFormElement")}}
    <ul>
      <li><a href="/en-US/docs/Web/API/HTMLFormElement/formdata_event">formdata event</a></li>
      <li><a href="/en-US/docs/Web/API/HTMLFormElement/reset_event">reset event</a></li>
      <li><a href="/en-US/docs/Web/API/HTMLFormElement/submit_event">submit event</a></li>
    </ul>
  </li>
  <li>{{DOMxRef("HTMLInputElement")}}
    <ul>
      <li><a href="/en-US/docs/Web/API/HTMLInputElement/invalid_event">invalid event</a></li>
      <li><a href="/en-US/docs/Web/API/HTMLInputElement/search_event">search event</a></li>
    </ul>
  </li>
  <li>{{DOMxRef("HTMLMediaElement")}}
    <ul>
      <li><a href="/en-US/docs/Web/API/HTMLMediaElement/abort_event">abort event</a></li>
      <li><a href="/en-US/docs/Web/API/HTMLMediaElement/canplaythrough_event">canplaythrough event</a></li>
      <li><a href="/en-US/docs/Web/API/HTMLMediaElement/canplay_event">canplay event</a></li>
      <li><a href="/en-US/docs/Web/API/HTMLMediaElement/durationchange_event">durationchange event</a></li>
      <li><a href="/en-US/docs/Web/API/HTMLMediaElement/emptied_event">emptied event</a></li>
      <li><a href="/en-US/docs/Web/API/HTMLMediaElement/ended_event">ended event</a></li>
      <li><a href="/en-US/docs/Web/API/HTMLMediaElement/error_event">error event</a></li>
      <li><a href="/en-US/docs/Web/API/HTMLMediaElement/loadeddata_event">loadeddata event</a></li>
      <li><a href="/en-US/docs/Web/API/HTMLMediaElement/loadedmetadata_event">loadedmetadata event</a></li>
      <li><a href="/en-US/docs/Web/API/HTMLMediaElement/loadstart_event">loadstart event</a></li>
      <li><a href="/en-US/docs/Web/API/HTMLMediaElement/pause_event">pause event</a></li>
      <li><a href="/en-US/docs/Web/API/HTMLMediaElement/playing_event">playing event</a></li>
      <li><a href="/en-US/docs/Web/API/HTMLMediaElement/play_event">play event</a></li>
      <li><a href="/en-US/docs/Web/API/HTMLMediaElement/progress_event">progress event</a></li>
      <li><a href="/en-US/docs/Web/API/HTMLMediaElement/ratechange_event">ratechange event</a></li>
      <li><a href="/en-US/docs/Web/API/HTMLMediaElement/seeked_event">seeked event</a></li>
      <li><a href="/en-US/docs/Web/API/HTMLMediaElement/seeking_event">seeking event</a></li>
      <li><a href="/en-US/docs/Web/API/HTMLMediaElement/stalled_event">stalled event</a></li>
      <li><a href="/en-US/docs/Web/API/HTMLMediaElement/suspend_event">suspend event</a></li>
      <li><a href="/en-US/docs/Web/API/HTMLMediaElement/timeupdate_event">timeupdate event</a></li>
      <li><a href="/en-US/docs/Web/API/HTMLMediaElement/volumechange_event">volumechange event</a></li>
      <li><a href="/en-US/docs/Web/API/HTMLMediaElement/waiting_event">waiting event</a></li>
    </ul>
  </li>
  <li>{{DOMxRef("HTMLSlotElement")}}
    <ul>
      <li><a href="/en-US/docs/Web/API/HTMLSlotElement/slotchange_event">slotchange event</a></li>
    </ul>
  </li>
  <li>{{DOMxRef("HTMLTrackElement")}}
    <ul>
      <li><a href="/en-US/docs/Web/API/HTMLTrackElement/cuechange_event">cuechange event</a></li>
    </ul>
  </li>
  <li>{{DOMxRef("HTMLVideoElement")}}
    <ul>
      <li><a href="/en-US/docs/Web/API/HTMLVideoElement/enterpictureinpicture_event">enterpictureinpicture event</a></li>
      <li><a href="/en-US/docs/Web/API/HTMLVideoElement/leavepictureinpicture_event">leavepictureinpicture event</a></li>
    </ul>
  </li>
  <li>{{DOMxRef("IDBDatabase")}}
    <ul>
      <li><a href="/en-US/docs/Web/API/IDBDatabase/abort_event">abort event</a></li>
      <li><a href="/en-US/docs/Web/API/IDBDatabase/close_event">close event</a></li>
      <li><a href="/en-US/docs/Web/API/IDBDatabase/error_event">error event</a></li>
      <li><a href="/en-US/docs/Web/API/IDBDatabase/versionchange_event">versionchange event</a></li>
    </ul>
  </li>
  <li>{{DOMxRef("IDBOpenDBRequest")}}
    <ul>
      <li><a href="/en-US/docs/Web/API/IDBOpenDBRequest/blocked_event">blocked event</a></li>
      <li><a href="/en-US/docs/Web/API/IDBOpenDBRequest/upgradeneeded_event">upgradeneeded event</a></li>
    </ul>
  </li>
  <li>{{DOMxRef("IDBRequest")}}
    <ul>
      <li><a href="/en-US/docs/Web/API/IDBRequest/error_event">error event</a></li>
      <li><a href="/en-US/docs/Web/API/IDBRequest/success_event">success event</a></li>
    </ul>
  </li>
  <li>{{DOMxRef("IDBTransaction")}}
    <ul>
      <li><a href="/en-US/docs/Web/API/IDBTransaction/abort_event">abort event</a></li>
      <li><a href="/en-US/docs/Web/API/IDBTransaction/complete_event">complete event</a></li>
      <li><a href="/en-US/docs/Web/API/IDBTransaction/error_event">error event</a></li>
    </ul>
  </li>
  <li>{{DOMxRef("MediaDevices")}}
    <ul>
      <li><a href="/en-US/docs/Web/API/MediaDevices/devicechange_event">devicechange event</a></li>
    </ul>
  </li>
  <li>{{DOMxRef("MediaRecorder")}}
    <ul>
      <li><a href="/en-US/docs/Web/API/MediaRecorder/error_event">error event</a></li>
    </ul>
  </li>
  <li>{{DOMxRef("MediaStream")}}
    <ul>
      <li><a href="/en-US/docs/Web/API/MediaStream/addtrack_event">addtrack event</a></li>
      <li><a href="/en-US/docs/Web/API/MediaStream/removetrack_event">removetrack event</a></li>
    </ul>
  </li>
  <li>{{DOMxRef("MediaStreamTrack")}}
    <ul>
      <li><a href="/en-US/docs/Web/API/MediaStreamTrack/ended_event">ended event</a></li>
      <li><a href="/en-US/docs/Web/API/MediaStreamTrack/mute_event">mute event</a></li>
      <li><a href="/en-US/docs/Web/API/MediaStreamTrack/unmute_event">unmute event</a></li>
    </ul>
  </li>
  <li>{{DOMxRef("MessagePort")}}
    <ul>
      <li><a href="/en-US/docs/Web/API/MessagePort/messageerror_event">messageerror event</a></li>
      <li><a href="/en-US/docs/Web/API/MessagePort/message_event">message event</a></li>
    </ul>
  </li>
  <li>{{DOMxRef("OfflineAudioContext")}}
    <ul>
      <li><a href="/en-US/docs/Web/API/OfflineAudioContext/complete_event">complete event</a></li>
    </ul>
  </li>
  <li>{{DOMxRef("PaymentRequest")}}
    <ul>
      <li><a href="/en-US/docs/Web/API/PaymentRequest/merchantvalidation_event">merchantvalidation event</a></li>
      <li><a href="/en-US/docs/Web/API/PaymentRequest/paymentmethodchange_event">paymentmethodchange event</a></li>
      <li><a href="/en-US/docs/Web/API/PaymentRequest/shippingaddresschange_event">shippingaddresschange event</a></li>
      <li><a href="/en-US/docs/Web/API/PaymentRequest/shippingoptionchange_event">shippingoptionchange event</a></li>
    </ul>
  </li>
  <li>{{DOMxRef("PaymentResponse")}}
    <ul>
      <li><a href="/en-US/docs/Web/API/PaymentResponse/payerdetailchange_event">payerdetailchange event</a></li>
    </ul>
  </li>
  <li>{{DOMxRef("Performance")}}
    <ul>
      <li><a href="/en-US/docs/Web/API/Performance/resourcetimingbufferfull_event">resourcetimingbufferfull event</a></li>
    </ul>
  </li>
  <li>{{DOMxRef("PictureInPictureWindow")}}
    <ul>
      <li><a href="/en-US/docs/Web/API/PictureInPictureWindow/resize_event">resize event</a></li>
    </ul>
  </li>
  <li>{{DOMxRef("RTCDataChannel")}}
    <ul>
      <li><a href="/en-US/docs/Web/API/RTCDataChannel/bufferedamountlow_event">bufferedamountlow event</a></li>
      <li><a href="/en-US/docs/Web/API/RTCDataChannel/close_event">close event</a></li>
      <li><a href="/en-US/docs/Web/API/RTCDataChannel/closing_event">closing event</a></li>
      <li><a href="/en-US/docs/Web/API/RTCDataChannel/error_event">error event</a></li>
      <li><a href="/en-US/docs/Web/API/RTCDataChannel/message_event">message event</a></li>
      <li><a href="/en-US/docs/Web/API/RTCDataChannel/open_event">open event</a></li>
    </ul>
  </li>
  <li>{{DOMxRef("RTCDtlsTransport")}}
    <ul>
      <li><a href="/en-US/docs/Web/API/RTCDtlsTransport/error_event">error event</a></li>
    </ul>
  </li>
  <li>{{DOMxRef("RTCDTMFSender")}}
    <ul>
      <li><a href="/en-US/docs/Web/API/RTCDTMFSender/tonechange_event">tonechange event</a></li>
    </ul>
  </li>
  <li>{{DOMxRef("RTCIceTransport")}}
    <ul>
      <li><a href="/en-US/docs/Web/API/RTCIceTransport/gatheringstatechange_event">gatheringstatechange event</a></li>
      <li><a href="/en-US/docs/Web/API/RTCIceTransport/selectedcandidatepairchange_event">selectedcandidatepairchange event</a></li>
      <li><a href="/en-US/docs/Web/API/RTCIceTransport/statechange_event">statechange event</a></li>
    </ul>
  </li>
  <li>{{DOMxRef("RTCPeerConnection")}}
    <ul>
      <li><a href="/en-US/docs/Web/API/RTCPeerConnection/addstream_event">addstream event</a></li>
      <li><a href="/en-US/docs/Web/API/RTCPeerConnection/connectionstatechange_event">connectionstatechange event</a></li>
      <li><a href="/en-US/docs/Web/API/RTCPeerConnection/datachannel_event">datachannel event</a></li>
      <li><a href="/en-US/docs/Web/API/RTCPeerConnection/icecandidateerror_event">icecandidateerror event</a></li>
      <li><a href="/en-US/docs/Web/API/RTCPeerConnection/icecandidate_event">icecandidate event</a></li>
      <li><a href="/en-US/docs/Web/API/RTCPeerConnection/iceconnectionstatechange_event">iceconnectionstatechange event</a></li>
      <li><a href="/en-US/docs/Web/API/RTCPeerConnection/icegatheringstatechange_event">icegatheringstatechange event</a></li>
      <li><a href="/en-US/docs/Web/API/RTCPeerConnection/negotiationneeded_event">negotiationneeded event</a></li>
      <li><a href="/en-US/docs/Web/API/RTCPeerConnection/removestream_event">removestream event</a></li>
      <li><a href="/en-US/docs/Web/API/RTCPeerConnection/signalingstatechange_event">signalingstatechange event</a></li>
      <li><a href="/en-US/docs/Web/API/RTCPeerConnection/track_event">track event</a></li>
    </ul>
  </li>
  <li>{{DOMxRef("ScriptProcessorNode")}}
    <ul>
      <li><a href="/en-US/docs/Web/API/ScriptProcessorNode/audioprocess_event">audioprocess event</a></li>
    </ul>
  </li>
  <li>{{DOMxRef("ServiceWorkerContainer")}}
    <ul>
      <li><a href="/en-US/docs/Web/API/ServiceWorkerContainer/message_event">message event</a></li>
    </ul>
  </li>
  <li>{{DOMxRef("ServiceWorkerGlobalScope")}}
    <ul>
      <li><a href="/en-US/docs/Web/API/ServiceWorkerGlobalScope/activate_event">activate event</a></li>
      <li><a href="/en-US/docs/Web/API/ServiceWorkerGlobalScope/contentdelete_event">contentdelete event</a></li>
      <li><a href="/en-US/docs/Web/API/ServiceWorkerGlobalScope/install_event">install event</a></li>
      <li><a href="/en-US/docs/Web/API/ServiceWorkerGlobalScope/message_event">message event</a></li>
      <li><a href="/en-US/docs/Web/API/ServiceWorkerGlobalScope/notificationclick_event">notificationclick event</a></li>
      <li><a href="/en-US/docs/Web/API/ServiceWorkerGlobalScope/pushsubscriptionchange_event">pushsubscriptionchange event</a></li>
      <li><a href="/en-US/docs/Web/API/ServiceWorkerGlobalScope/push_event">push event</a></li>
    </ul>
  </li>
  <li>{{DOMxRef("SharedWorkerGlobalScope")}}
    <ul>
      <li><a href="/en-US/docs/Web/API/SharedWorkerGlobalScope/connect_event">connect event</a></li>
    </ul>
  </li>
  <li>{{DOMxRef("SpeechRecognition")}}
    <ul>
      <li><a href="/en-US/docs/Web/API/SpeechRecognition/audioend_event">audioend event</a></li>
      <li><a href="/en-US/docs/Web/API/SpeechRecognition/audiostart_event">audiostart event</a></li>
      <li><a href="/en-US/docs/Web/API/SpeechRecognition/end_event">end event</a></li>
      <li><a href="/en-US/docs/Web/API/SpeechRecognition/error_event">error event</a></li>
      <li><a href="/en-US/docs/Web/API/SpeechRecognition/nomatch_event">nomatch event</a></li>
      <li><a href="/en-US/docs/Web/API/SpeechRecognition/result_event">result event</a></li>
      <li><a href="/en-US/docs/Web/API/SpeechRecognition/soundend_event">soundend event</a></li>
      <li><a href="/en-US/docs/Web/API/SpeechRecognition/soundstart_event">soundstart event</a></li>
      <li><a href="/en-US/docs/Web/API/SpeechRecognition/speechend_event">speechend event</a></li>
      <li><a href="/en-US/docs/Web/API/SpeechRecognition/speechstart_event">speechstart event</a></li>
      <li><a href="/en-US/docs/Web/API/SpeechRecognition/start_event">start event</a></li>
    </ul>
  </li>
  <li>{{DOMxRef("SpeechSynthesis")}}
    <ul>
      <li><a href="/en-US/docs/Web/API/SpeechSynthesis/voiceschanged_event">voiceschanged event</a></li>
    </ul>
  </li>
  <li>{{DOMxRef("SpeechSynthesisUtterance")}}
    <ul>
      <li><a href="/en-US/docs/Web/API/SpeechSynthesisUtterance/boundary_event">boundary event</a></li>
      <li><a href="/en-US/docs/Web/API/SpeechSynthesisUtterance/end_event">end event</a></li>
      <li><a href="/en-US/docs/Web/API/SpeechSynthesisUtterance/error_event">error event</a></li>
      <li><a href="/en-US/docs/Web/API/SpeechSynthesisUtterance/mark_event">mark event</a></li>
      <li><a href="/en-US/docs/Web/API/SpeechSynthesisUtterance/pause_event">pause event</a></li>
      <li><a href="/en-US/docs/Web/API/SpeechSynthesisUtterance/resume_event">resume event</a></li>
      <li><a href="/en-US/docs/Web/API/SpeechSynthesisUtterance/start_event">start event</a></li>
    </ul>
  </li>
  <li>{{DOMxRef("SVGAnimationElement")}}
    <ul>
      <li><a href="/en-US/docs/Web/API/SVGAnimationElement/beginEvent_event">beginEvent event</a></li>
      <li><a href="/en-US/docs/Web/API/SVGAnimationElement/endEvent_event">endEvent event</a></li>
      <li><a href="/en-US/docs/Web/API/SVGAnimationElement/repeatEvent_event">repeatEvent event</a></li>
    </ul>
  </li>
  <li>{{DOMxRef("SVGElement")}}
    <ul>
      <li><a href="/en-US/docs/Web/API/SVGElement/abort_event">abort event</a></li>
      <li><a href="/en-US/docs/Web/API/SVGElement/error_event">error event</a></li>
      <li><a href="/en-US/docs/Web/API/SVGElement/load_event">load event</a></li>
      <li><a href="/en-US/docs/Web/API/SVGElement/resize_event">resize event</a></li>
      <li><a href="/en-US/docs/Web/API/SVGElement/scroll_event">scroll event</a></li>
      <li><a href="/en-US/docs/Web/API/SVGElement/unload_event">unload event</a></li>
    </ul>
  </li>
  <li>{{DOMxRef("SVGGraphicsElement")}}
    <ul>
      <li><a href="/en-US/docs/Web/API/SVGGraphicsElement/copy_event">copy event</a></li>
      <li><a href="/en-US/docs/Web/API/SVGGraphicsElement/cut_event">cut event</a></li>
      <li><a href="/en-US/docs/Web/API/SVGGraphicsElement/paste_event">paste event</a></li>
    </ul>
  </li>
  <li>{{DOMxRef("TextTrack")}}
    <ul>
      <li><a href="/en-US/docs/Web/API/TextTrack/cuechange_event">cuechange event</a></li>
    </ul>
  </li>
  <li>{{DOMxRef("TextTrackList")}}
    <ul>
      <li><a href="/en-US/docs/Web/API/TextTrackList/addtrack_event">addtrack event</a></li>
      <li><a href="/en-US/docs/Web/API/TextTrackList/change_event">change event</a></li>
      <li><a href="/en-US/docs/Web/API/TextTrackList/removeTrack_event">removeTrack event</a></li>
    </ul>
  </li>
  <li>{{DOMxRef("VideoTrackList")}}
    <ul>
      <li><a href="/en-US/docs/Web/API/VideoTrackList/addtrack_event">addtrack event</a></li>
      <li><a href="/en-US/docs/Web/API/VideoTrackList/change_event">change event</a></li>
      <li><a href="/en-US/docs/Web/API/VideoTrackList/removetrack_event">removetrack event</a></li>
    </ul>
  </li>
  <li>{{DOMxRef("VisualViewport")}}
    <ul>
      <li><a href="/en-US/docs/Web/API/VisualViewport/resize_event">resize event</a></li>
      <li><a href="/en-US/docs/Web/API/VisualViewport/scroll_event">scroll event</a></li>
    </ul>
  </li>
  <li>{{DOMxRef("WebSocket")}}
    <ul>
      <li><a href="/en-US/docs/Web/API/WebSocket/close_event">close event</a></li>
      <li><a href="/en-US/docs/Web/API/WebSocket/error_event">error event</a></li>
      <li><a href="/en-US/docs/Web/API/WebSocket/message_event">message event</a></li>
      <li><a href="/en-US/docs/Web/API/WebSocket/open_event">open event</a></li>
    </ul>
  </li>
  <li>{{DOMxRef("Window")}}
    <ul>
      <li><a href="/en-US/docs/Web/API/Window/afterprint_event">afterprint event</a></li>
      <li><a href="/en-US/docs/Web/API/Window/animationcancel_event">animationcancel event</a></li>
      <li><a href="/en-US/docs/Web/API/Window/animationend_event">animationend event</a></li>
      <li><a href="/en-US/docs/Web/API/Window/animationiteration_event">animationiteration event</a></li>
      <li><a href="/en-US/docs/Web/API/Window/animationstart_event">animationstart event</a></li>
      <li><a href="/en-US/docs/Web/API/Window/appinstalled_event">appinstalled event</a></li>
      <li><a href="/en-US/docs/Web/API/Window/beforeprint_event">beforeprint event</a></li>
      <li><a href="/en-US/docs/Web/API/Window/beforeunload_event">beforeunload event</a></li>
      <li><a href="/en-US/docs/Web/API/Window/blur_event">blur event</a></li>
      <li><a href="/en-US/docs/Web/API/Window/copy_event">copy event</a></li>
      <li><a href="/en-US/docs/Web/API/Window/cut_event">cut event</a></li>
      <li><a href="/en-US/docs/Web/API/Window/devicemotion_event">devicemotion event</a></li>
      <li><a href="/en-US/docs/Web/API/Window/deviceorientation_event">deviceorientation event</a></li>
      <li><a href="/en-US/docs/Web/API/Window/DOMContentLoaded_event">DOMContentLoaded event</a></li>
      <li><a href="/en-US/docs/Web/API/Window/error_event">error event</a></li>
      <li><a href="/en-US/docs/Web/API/Window/focus_event">focus event</a></li>
      <li><a href="/en-US/docs/Web/API/Window/gamepadconnected_event">gamepadconnected event</a></li>
      <li><a href="/en-US/docs/Web/API/Window/gamepaddisconnected_event">gamepaddisconnected event</a></li>
      <li><a href="/en-US/docs/Web/API/Window/hashchange_event">hashchange event</a></li>
      <li><a href="/en-US/docs/Web/API/Window/languagechange_event">languagechange event</a></li>
      <li><a href="/en-US/docs/Web/API/Window/load_event">load event</a></li>
      <li><a href="/en-US/docs/Web/API/Window/messageerror_event">messageerror event</a></li>
      <li><a href="/en-US/docs/Web/API/Window/message_event">message event</a></li>
      <li><a href="/en-US/docs/Web/API/Window/offline_event">offline event</a></li>
      <li><a href="/en-US/docs/Web/API/Window/online_event">online event</a></li>
      <li><a href="/en-US/docs/Web/API/Window/orientationchange_event">orientationchange event</a></li>
      <li><a href="/en-US/docs/Web/API/Window/pagehide_event">pagehide event</a></li>
      <li><a href="/en-US/docs/Web/API/Window/pageshow_event">pageshow event</a></li>
      <li><a href="/en-US/docs/Web/API/Window/paste_event">paste event</a></li>
      <li><a href="/en-US/docs/Web/API/Window/popstate_event">popstate event</a></li>
      <li><a href="/en-US/docs/Web/API/Window/rejectionhandled_event">rejectionhandled event</a></li>
      <li><a href="/en-US/docs/Web/API/Window/resize_event">resize event</a></li>
      <li><a href="/en-US/docs/Web/API/Window/storage_event">storage event</a></li>
      <li><a href="/en-US/docs/Web/API/Window/transitioncancel_event">transitioncancel event</a></li>
      <li><a href="/en-US/docs/Web/API/Window/transitionend_event">transitionend event</a></li>
      <li><a href="/en-US/docs/Web/API/Window/transitionrun_event">transitionrun event</a></li>
      <li><a href="/en-US/docs/Web/API/Window/transitionstart_event">transitionstart event</a></li>
      <li><a href="/en-US/docs/Web/API/Window/unhandledrejection_event">unhandledrejection event</a></li>
      <li><a href="/en-US/docs/Web/API/Window/unload_event">unload event</a></li>
      <li><a href="/en-US/docs/Web/API/Window/vrdisplayactivate_event">vrdisplayactivate event</a></li>
      <li><a href="/en-US/docs/Web/API/Window/vrdisplayblur_event">vrdisplayblur event</a></li>
      <li><a href="/en-US/docs/Web/API/Window/vrdisplayconnect_event">vrdisplayconnect event</a></li>
      <li><a href="/en-US/docs/Web/API/Window/vrdisplaydeactivate_event">vrdisplaydeactivate event</a></li>
      <li><a href="/en-US/docs/Web/API/Window/vrdisplaydisconnect_event">vrdisplaydisconnect event</a></li>
      <li><a href="/en-US/docs/Web/API/Window/vrdisplayfocus_event">vrdisplayfocus event</a></li>
      <li><a href="/en-US/docs/Web/API/Window/vrdisplaypointerrestricted_event">vrdisplaypointerrestricted event</a></li>
      <li><a href="/en-US/docs/Web/API/Window/vrdisplaypointerunrestricted_event">vrdisplaypointerunrestricted event</a></li>
      <li><a href="/en-US/docs/Web/API/Window/vrdisplaypresentchange_event">vrdisplaypresentchange event</a></li>
    </ul>
  </li>
  <li>{{DOMxRef("Worker")}}
    <ul>
      <li><a href="/en-US/docs/Web/API/Worker/messageerror_event">messageerror event</a></li>
      <li><a href="/en-US/docs/Web/API/Worker/message_event">message event</a></li>
    </ul>
  </li>
  <li>{{DOMxRef("WorkerGlobalScope")}}
    <ul>
      <li><a href="/en-US/docs/Web/API/WorkerGlobalScope/languagechange_event">languagechange event</a></li>
    </ul>
  </li>
  <li>{{DOMxRef("XMLHttpRequest")}}
    <ul>
      <li><a href="/en-US/docs/Web/API/XMLHttpRequest/abort_event">abort event</a></li>
      <li><a href="/en-US/docs/Web/API/XMLHttpRequest/error_event">error event</a></li>
      <li><a href="/en-US/docs/Web/API/XMLHttpRequest/loadend_event">loadend event</a></li>
      <li><a href="/en-US/docs/Web/API/XMLHttpRequest/loadstart_event">loadstart event</a></li>
      <li><a href="/en-US/docs/Web/API/XMLHttpRequest/load_event">load event</a></li>
      <li><a href="/en-US/docs/Web/API/XMLHttpRequest/progress_event">progress event</a></li>
      <li><a href="/en-US/docs/Web/API/XMLHttpRequest/timeout_event">timeout event</a></li>
    </ul>
  </li>
  <li>{{DOMxRef("XRReferenceSpace")}}
    <ul>
      <li><a href="/en-US/docs/Web/API/XRReferenceSpace/reset_event">reset event</a></li>
    </ul>
  </li>
  <li>{{DOMxRef("XRSession")}}
    <ul>
      <li><a href="/en-US/docs/Web/API/XRSession/end_event">end event</a></li>
      <li><a href="/en-US/docs/Web/API/XRSession/inputsourceschange_event">inputsourceschange event</a></li>
      <li><a href="/en-US/docs/Web/API/XRSession/selectend_event">selectend event</a></li>
      <li><a href="/en-US/docs/Web/API/XRSession/selectstart_event">selectstart event</a></li>
      <li><a href="/en-US/docs/Web/API/XRSession/select_event">select event</a></li>
      <li><a href="/en-US/docs/Web/API/XRSession/squeezeend_event">squeezeend event</a></li>
      <li><a href="/en-US/docs/Web/API/XRSession/squeezestart_event">squeezestart event</a></li>
      <li><a href="/en-US/docs/Web/API/XRSession/squeeze_event">squeeze event</a></li>
      <li><a href="/en-US/docs/Web/API/XRSession/visibilitychange_event">visibilitychange event</a></li>
    </ul>
  </li>
  <li>{{DOMxRef("XRSystem")}}
    <ul>
      <li><a href="/en-US/docs/Web/API/XRSystem/devicechange_event">devicechange event</a></li>
    </ul>
  </li>
</ul>


<h2 id="Specifications">Specifications</h2>

<table class="standard-table">
 <thead>
  <tr>
   <th scope="col">Specification</th>
   <th scope="col">Status</th>
   <th scope="col">Comment</th>
  </tr>
 </thead>
 <tbody>
  <tr>
   <td>{{SpecName('HTML WHATWG', 'webappapis.html#event-handler-attributes', 'event handlers')}}</td>
   <td>{{Spec2('HTML WHATWG')}}</td>
   <td></td>
  </tr>
  <tr>
   <td>{{SpecName('HTML5 W3C', 'webappapis.html#event-handler-attributes', 'event handlers')}}</td>
   <td>{{Spec2('HTML5 W3C')}}</td>
   <td></td>
  </tr>
 </tbody>
</table>

<section id="Quick_links">
  <ul>
    <li><a href="/en-US/docs/Learn/JavaScript/Building_blocks/Events">Introduction to events</a></li>
  </ul>
  {{ListSubpages}}
 </section>