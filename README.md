# OpenSmartArray
OpenSmartArray is a intelligent storage box to support big data storage application. It can support different type of interface including
object storage interface, traditional storage interface like block interface, posix interface etc. It will take advantage most
advantage hardware in the world like NVMe device, optone device. The storage stack was built to totally release the power of hardware.
It gets rid of traditional software storage bottleneck. It has both SDS and HCI features. It will has snapshot, dedupe, compression features for SDS with computing resources in place(data locality support with tiering support). In the same time, we support data portability for computing platform like container. 

In terms of computing platform , we are going to choose container/docker as our major computing platform. 

User space driver platform DPDK will be choosed as major platform since it provide best IOPS/cpu utilization as well as CPU latency.
NVMe over RDMA fabrics (also in user space)will be choosed as major connection to connect with outside. We are going to develop target driver in user space for NVMe over RDMA fabrics.XIO messager is going to directly talk with NVMe over RDMA fabrics.



