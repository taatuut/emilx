# emilx
MLX experiments

mlxserver
---

https://github.com/mustafaaljadery/mlxserver

```
python3 -m pip install mlxserver

create emilxserver.py

python3 emilxserver.py

curl -X GET 'http://127.0.0.1:5000/generate?prompt=write%20me%20a%20poem%20about%20Solace%20PubSub%20platform%20for%20Event-Driven%20Architecture&stream=true'
```

Answer:
> Solace PubSub+, a platform built to last,
> A solution for event-driven architecture, it's a blast!
> 
> With Solace, we can send and receive messages with ease,
> Using APIs, we can integrate with any system with no fuss or freeze.
> 
> Solace PubSub+, a platform that's reliable and fast,
> It's the perfect solution for event-driven architecture, it's a blast!
> 
> Solace's event brokers are built to handle high volume traffic,
> With low latency and high throughput, it's a match!
> 
> Solace PubSub+, a platform that's secure and scalable,
> It's the perfect solution for event-driven architecture, it's a fable!
> 
> Solace's event brokers can be deployed on-prem or in the cloud,
> With Solace, we can build a system that's always around.
> 
> Solace PubSub+, a platform that's easy to use and manage,
> It's the perfect solution for event-driven architecture, it's a range!
> 
> With Solace, we can build a system that's flexible and agile,
> It's the perfect solution for event-driven architecture, it's a mile!
> 
> Solace PubSub+, a platform that's built to last,
> It's the perfect solution for event-driven architecture, it's a blast!

MLX RAG
---

https://github.com/vegaluisjose/mlx-rag

```
python3 -m pip install mlx==0.0.10 mlx-lm==0.0.3 pydantic unstructured pdf2image pdfminer.six pillow pillow_heif opencv-python pytesseract pikepdf

python3 -m pip uninstall pdfminer

python3 create_vdb.py --pdf "/Users/emilzegers/GitHub/taatuut/clear-agnostic/docs/SolacePubsub+DistributedTracing.pdf" --vdb vdb.npz

python3 query_vdb.py --question "what is distributed tracing?"
```

Answer:
> Distributed tracing is an approach to monitor and analyze the performance of a complex, distributed system in real-time, providing a comprehensive view of the user experience from the application layer to the underlying infrastructure. It helps developers quickly identify and resolve issues by offering root cause analysis data.

`python3 query_vdb.py --question "how does solace pubsub+ platform support observability?"`

Answer:
> Solace PubSub+ Distributed Tracing supports observability through OpenTelemetry, providing real-time data about message and event status in a complex microservices environment or event-driven architecture. This data is then delivered to the user's chosen observability tools.

`python3 query_vdb.py --question "what is the business value of Distributed Tracing for Solace PubSub+?"`

Answer:
> The business value of Distributed Tracing for Solace PubSub+ includes real-time insights into core business processes, enabling organizations to monitor complex microservices and event-driven architectures, satisfy regulatory and audit compliance, and quickly respond to issues with relevant root cause analysis data. This helps improve efficiency, reduce downtime, and ensure compliance.
