# P2P Mesh Network Simulation with NS-3

A 10-node ad-hoc wireless network simulation where nodes periodically exchange UDP "shares".

## 🛠️ Setup

```bash
# Clone THIS repository
git clone https://github.com/asmit27rai/p2p-mesh-ns3.git
cd p2p-mesh-ns3

# Install NS-3
git clone https://gitlab.com/nsnam/ns-3-dev.git
cd ns-3-dev
./ns3 configure --enable-examples
./ns3 build

# From ns-3-dev directory
ln -s ../../my-simulations/p2p-mesh scratch/

# From ns-3-dev directory
./ns3 run scratch/p2p-mesh/p2p-mesh.cc

```

## ✅ Expected Output
### You should see periodic messages like:

```bash
At time +1.000s OnOffApplication sending packet to 10.1.1.2
At time +2.000s OnOffApplication sending packet to 10.1.1.3
...
At time +20.000s Simulation stopped
```

