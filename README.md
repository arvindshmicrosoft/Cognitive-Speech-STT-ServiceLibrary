# Cognitive-Speech-STT-ServiceLibrary
Service SDK - C# Samples, documentation for service to service speech to text

This fork by Arvind Shyamsundar is a Class Library version which can then be invoked from other clients, including Python (using PyDotNet). Sample with Python 3.5.2 as shown below (first you do need to install PyDotNet for Python 3.5 - refer to https://bitbucket.org/pydotnet/pydotnet/wiki/Home)

Here's the Python sample:

import dotnet.seamless
dotnet.add_assemblies(r"<< Folder Path to where you built SpeechClientSample.dll but NO file name ")
dotnet.load_assembly("SpeechClientSample")
from SpeechClientSample import SpeechAPIWrapper
SpeechAPIWrapper.InvokeBingSpeechWebSocketAPI(r" <<Full path to .WAV file including file name>> ", "en-US", "Long", r"<<API_KEY>>")
