# Mind the Gap
[![CircleCI Build Status](https://circleci.com/gh/james-crowley/mind-the-gap.svg?style=shield)](https://circleci.com/gh/james-crowley/mind-the-gap) [![Software License](https://img.shields.io/badge/license-MIT-blue.svg)](https://raw.githubusercontent.com/james-crowley/mind-the-gap/main/LICENSE) [![Docker Pulls](https://img.shields.io/docker/pulls/jimcrowley/mind-the-gap-demo)](https://hub.docker.com/r/jimcrowley/mind-the-gap-demo)


This demo aims to show users how to bridge the "gap" between their own networks and CircleCI's network. 


Bridging the gap is useful when users have similar use cases to these:

- Accessing private artifact repositories
- Pulling dependencies from behind a firewall
- Running test cases on an internal environment
- Performing integration testing against private cloud resources
- Deploying an internal app with sensitive data
- Granting access to a production network

Currently, there are 3 primary ways to the bridge the gap with CircleCI:

- Running a [VPN](https://circleci.com/developer/orbs/orb/titel-media/openvpn) or [overlay network](https://circleci.com/developer/orbs/orb/crowley-namespace/tailscale)
- Deploy a self-hosted [Runner](https://circleci.com/docs/2.0/runner-overview/) installed within a private network
- Utilizing [IP Ranges](https://circleci.com/docs/2.0/ip-ranges/) which provides a list of well-defined IP address ranges associated with the CircleCI service


Each method of bridging the gap has pros and cons. Depending on the users use case they might prefer one method over
the other. 

At the end of this demo, users should have a better understanding of each method and which method might suits their needs the best.


