ns3-gym
============

OpenAI Gym is a toolkit for reinforcement learning widely used in research. The ns–3 network simulator is the de–facto standard for academic and industry research into networking protocols and communications technology. Ns3-gym is a framework which integrates OpenAI Gym into ns-3.

Installation
============

0. Switch branch to gym:

		git checkout gym

1. Install all required dependencies required by ns-3.

		# minimal requirements for C++:
		apt-get install gcc g++ python

		see https://www.nsnam.org/wiki/Installation

2. Install ZMQ and Protocol Buffers libs:

		# to install protobuf-3.6 on ubuntu 16.04:
		sudo add-apt-repository ppa:maarten-fonville/protobuf
		sudo apt-get update

		apt-get install libzmq5 libzmq5-dev
		apt-get install libprotobuf-dev
		apt-get install protobuf-compiler

3. Install PyOpenGymNs3 located in src/opengym/model/PyOpenGymNs3 (Python3 required)

		pip3 install ./src/opengym/model/PyOpenGymNs3

4. Configure and build ns-3 project:

		# Opengym Protobuf messages are build during configure
		./waf configure
		./waf

5. (Optional) Install all libraries required by your agent (like tensorflow, keras, etc.).

6. Run example:

		cd ./scratch/opengym
		./simple_test.py

Contact
============
* Piotr Gawlowicz, TU-Berlin, gawlowicz@tkn
* Anatolij Zubow, TU-Berlin, zubow@tkn
* tkn = tkn.tu-berlin.de

How to reference ns3-gym?
============

Please use the following bibtex :

```

```
