# Node.js Server Unresponsiveness with Long Delays

This repository demonstrates a common issue in Node.js servers: unresponsiveness due to long-running operations in request handlers.  The `serverBug.js` file shows a server that introduces a 5-second delay. During this delay, the server becomes unresponsive to new requests.

The `serverSolution.js` file provides a solution using the `cluster` module to handle multiple requests concurrently and prevent the server from hanging.