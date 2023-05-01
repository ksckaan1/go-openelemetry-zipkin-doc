# OpenTelemetry ve Golang

## OpenTelemetry Nedir?

OpenTelemetry, bulut tabanlı uygulamaların izlenmesi ve gözlemlemesi için bir araç setidir. Bu araçlar, dağıtılmış sistemlerde çalışan birden fazla hizmetin izlenmesini ve gözlenmesini sağlar.

OpenTelemetry, aşağıdaki ana bileşenlerden oluşur:

- **Collectors:** Veri toplama için kullanılan araçlardır. Hizmetlerden gelen izleme verilerini toplar ve işler.

- **SDKs:** Programlama dili için özelleştirilmiş yazılım geliştirme kütüphaneleridir. Hizmetlerin OpenTelemetry tarafından toplanan verileri üretmesine olanak tanır.

- **Exporters:** Verileri işlemek ve analiz etmek için farklı hizmetlere aktarmak için kullanılan araçlardır.

OpenTelemetry'nin farklı programlama dilleri için SDK'ları bulunmaktadır. Örneğin, Java, Python, Go, Ruby ve .NET için SDK'ları bulunmaktadır. Böylece, OpenTelemetry, birçok farklı dilde yazılmış uygulamaların izlenmesini ve gözlenmesini sağlar.

OpenTelemetry, bulut tabanlı uygulamaların izlenmesi için standart bir araç seti olma yolunda ilerlemektedir. Bu nedenle, birçok büyük bulut sağlayıcısı, OpenTelemetry'nin kullanımını desteklemektedir.

### OpenTelemetry Collectors
OpenTelemetry Collectors, OpenTelemetry ile uyumlu olan hizmetlerin verilerini toplayan, işleyen ve yöneten araçlardır. Collectors, OpenTelemetry'nin toplama katmanında bulunur ve diğer katmanlarla etkileşim halindedir.

Collectors, birden fazla veri kaynağından veri toplama işlemini kolaylaştırmak için tasarlanmıştır. Collectors, ayrıca gelen verileri filtreleyebilir, önbelleğe alabilir ve birden fazla hedefe gönderebilir. Bu hedefler, verilerin işlenmesi, analiz edilmesi ve depolanması için kullanılabilir.

Collectors, OpenTelemetry'nin toplama katmanında bulunur ve birden fazla veri kaynağından veri toplama işlemini kolaylaştırmak için tasarlanmıştır. Collectors, ayrıca gelen verileri filtreleyebilir, önbelleğe alabilir ve birden fazla hedefe gönderebilir. Bu hedefler, verilerin işlenmesi, analiz edilmesi ve depolanması için kullanılabilir.

OpenTelemetry, farklı veri kaynaklarından veri toplama işlemini kolaylaştırmak için birkaç farklı türde Collector sağlar:

- **Trace Collectors:** Dağıtılmış sistemlerdeki hizmetlerin etkinliklerini izler ve raporlar.

- **Metrics Collectors:** Hizmetlerin performans verilerini ölçer ve raporlar.

- **Logs Collectors:** Hizmetlerin günlük dosyalarını toplar ve raporlar.

OpenTelemetry'nin Collectors'ları, hizmetlerin izlenmesi ve gözlenmesi için kullanılan diğer araçlarla da entegre edilebilir. Örneğin, bir Collector, verileri bir gözlem paneline göndermek için bir Exporter kullanabilir.

### OpenTelemetry SDKs
OpenTelemetry SDK'ları, hizmetlerin izlenmesi ve gözlenmesi için kullanılan yazılım geliştirme kütüphaneleridir. Bu SDK'lar, belirli bir programlama dili için yazılmıştır ve OpenTelemetry'nin veri toplama katmanında bulunur. SDK'lar, hizmetlerin izleme verilerini OpenTelemetry Collectors'a göndermesini sağlar.

OpenTelemetry, şu anda birçok farklı programlama dili için SDK sağlamaktadır. Bu diller arasında Java, Python, Go, Ruby, .NET ve Node.js gibi popüler diller bulunur. Bu SDK'lar, hizmetlerin OpenTelemetry tarafından toplanan verileri üretmesine olanak tanır.

OpenTelemetry SDK'ları, izleme verilerini toplamak, filtrelemek, önbelleğe almak ve OpenTelemetry Exporters'a göndermek için kullanılabilir. SDK'lar ayrıca, hizmetlerin OpenTelemetry tarafından toplanan verilerini özelleştirmelerine olanak tanıyan bir dizi yapılandırma seçeneği sunar.

OpenTelemetry SDK'ları, hizmetlerin OpenTelemetry tarafından toplanan verileri üretmesini sağlar. Örneğin, bir OpenTelemetry Trace SDK'sı, hizmetin etkinliklerini izler ve raporlar. Bu izleme verileri, bir Collectors aracılığıyla OpenTelemetry Exporters'a gönderilebilir.

OpenTelemetry SDK'ları, hizmetlerin farklı bulut sağlayıcılarda çalışmasına izin verir. Bu sayede, farklı bulut sağlayıcılarda çalışan hizmetlerin izleme verileri birleştirilebilir ve tek bir yerde toplanabilir.

### OpenTelemetry Exporters

OpenTelemetry Exporter'ları, OpenTelemetry tarafından toplanan izleme verilerini çeşitli hedeflere göndermek için kullanılır. Bu hedefler arasında bulut sağlayıcıları, izleme araçları, günlük sistemleri ve diğer veri depolama sistemleri bulunur. Exporter'lar, OpenTelemetry'nin son aşamasında bulunur ve verileri dışa aktarmak için kullanılır.

Exporter'lar, OpenTelemetry tarafından toplanan verileri bir dizi farklı format ve protokolde göndermek için kullanılabilir. Bu formatlar arasında JSON, Protobuf ve OpenMetrics bulunur. Protokoller arasında HTTP, gRPC, TCP ve UDP gibi farklı seçenekler mevcuttur.

OpenTelemetry, birçok farklı hedefe veri göndermek için bir dizi hazır Exporter sağlar. Bu Exporter'lar, hizmetlerin izleme verilerini popüler bulut sağlayıcılarına, özel izleme araçlarına ve diğer veri depolama sistemlerine göndermek için kullanılabilir.

OpenTelemetry'nin Exporter'ları ayrıca özelleştirilebilir. Bu sayede, hizmetlerin izleme verileri belirli bir formatta ve protokolde gönderilebilir. Özelleştirilebilir Exporter'lar, hizmetlerin verileri belirli bir hedefe göndermek için gereksinimlerini karşılayacak şekilde yapılandırılabilir.

Örneğin, bir OpenTelemetry Trace Exporter'ı, hizmetin etkinliklerini izler ve raporlar. Bu veriler, OpenTelemetry tarafından toplandıktan sonra bir Exporter aracılığıyla bir hedefe gönderilebilir.

## OpenTelemetry Verilerini İzleme ve Analiz Etme

OpenTelemetry tarafından toplanan verileri izlemek ve analiz etmek için birçok farklı platform ve araç mevcuttur. Aşağıda, popüler OpenTelemetry veri gözlemleme platformlarının bazıları yer almaktadır:

- **Zipkin:** Zipkin, açık kaynaklı bir izleme sistemi ve hizmeti izlemek için kullanılan bir araçtır. Zipkin, hizmetlerin izleme verilerini görselleştirmek ve analiz etmek için kullanılır.

- **Grafana:** Grafana, hizmetlerin OpenTelemetry tarafından toplanan izleme verilerini görselleştirmek için kullanılan açık kaynaklı bir platformdur. Grafana, birden fazla veri kaynağından verileri toplayabilir ve izleme verilerini anlık olarak görüntüleyebilir.

- **Prometheus:** Prometheus, açık kaynaklı bir sistem izleme aracıdır ve OpenTelemetry verilerini analiz etmek için sıklıkla kullanılır. Prometheus, birden fazla hizmetin izleme verilerini toplar ve grafikler, uyarılar ve diğer ölçümler oluşturmak için kullanılabilir.

- **Jaeger:** Jaeger, açık kaynaklı bir izleme sistemi ve hizmeti izlemek için kullanılan bir araçtır. Jaeger, hizmetlerin izleme verilerini görselleştirmek ve analiz etmek için kullanılır.

- **New Relic:** New Relic, hizmetlerin performansını izlemek için kullanılan bir SaaS aracıdır. OpenTelemetry verilerini toplayabilir ve görselleştirebilir, böylece hizmet performansını anlık olarak izleyebilirsiniz.

- **Datadog:** Datadog, hizmetlerin izleme verilerini toplayan ve analiz eden bir SaaS platformudur. OpenTelemetry verilerini toplayabilir ve görselleştirebilir, böylece hizmet performansını anlık olarak izleyebilirsiniz.

- **Splunk:** Splunk, hizmetlerin izleme verilerini toplamak ve analiz etmek için kullanılan bir SaaS platformudur. OpenTelemetry verilerini toplayabilir ve görselleştirebilir, böylece hizmet performansını anlık olarak izleyebilirsiniz.

Bu, OpenTelemetry verilerini gözlemlemek için kullanabileceğiniz popüler platformlardan sadece birkaçıdır. Bunların yanı sıra, Elasticsearch, Kibana, Dynatrace ve daha birçok araç ve platform, OpenTelemetry verilerini izlemek için kullanılabilir.

## Zipkin

Zipkin, dağıtık sistemlerdeki mikro hizmetlerin izlenmesini sağlamak için kullanılan açık kaynaklı bir yazılım aracıdır. Zipkin, tüm işlemlerin bir izleme ağacında izlendiği bir yapıda çalışır. Bu sayede, bir işlemdeki tüm mikro hizmet çağrıları izlenebilir ve hatalı bir çağrının kökeni kolayca tespit edilebilir.

Zipkin, geleneksel istek yanıt izleme yöntemlerinden farklı olarak işlemler arasındaki bağlantıyı izlemek için izleme bağlamı (trace context) kullanır. Her işlem, benzersiz bir izleme kimliği (trace ID) ve her bir mikro hizmet çağrısı için bir span (araç) kimliği oluşturur. Span'lar, mikro hizmet çağrılarının süresi, hataları ve diğer ayrıntıları gibi çeşitli bilgileri içerir.

Zipkin, işlem izleme verilerini toplar, depolar ve görselleştirir. Bu sayede, sistemdeki performans sorunlarını veya hataları tespit etmek ve bunların kökenlerini izlemek kolaylaşır. Ayrıca, Zipkin, OpenTracing, OpenCensus ve OpenTelemetry gibi açık standartlarla uyumlu olduğundan, birçok dil ve platformda kullanılabilir.

# Go'da OpenTelemetry Verilerini Zipkin'den İzlemek için Örnek Bir Yapı

## Docker'da Zipkin'i Çalıştıralım

```shell
docker run -d -p 9411:9411 openzipkin/zipkin
```

Zipkin UI'da Trace'leri görmek için http://localhost:9411/zipkin/ adresine gidebilirsiniz.


## Go'da OpenTelemetry'nin ve Zipkin Exporter'ın Ayarlanması

> `tracer.go` dosyası
```go
package main

import (
	"context"
	"go.opentelemetry.io/otel"
	"go.opentelemetry.io/otel/exporters/zipkin"
	"go.opentelemetry.io/otel/sdk/resource"
	sdktrace "go.opentelemetry.io/otel/sdk/trace"
	semconv "go.opentelemetry.io/otel/semconv/v1.17.0"
	trace2 "go.opentelemetry.io/otel/trace"
	"log"
)

// programın geri kalanında kullanacailceğimiz Tracer nesnemiz
type Tracer struct {
	tp *sdktrace.TracerProvider
}

// Tracer oluştururken zipkin url'ini ve servis ismini veriyoruz
func NewTracer(url, serviceName string) (*Tracer, error) {
	// zipkin exporter'ını init edelim
	exporter, err := zipkin.New(url)
	if err != nil {
		return nil, err
	}

	// veri kaynağının tanıtılması
	res, err := resource.New(
		context.Background(),
		resource.WithAttributes(
			// the service name used to display traces in backends
			semconv.ServiceNameKey.String(serviceName),
		),
	)
	if err != nil {
		log.Fatalf("unable to initialize resource due: %v", err)
	}
	
	// trace sağlayıcının tanımlanması
	tp := sdktrace.NewTracerProvider(
		sdktrace.WithSampler(sdktrace.AlwaysSample()),
		sdktrace.WithBatcher(exporter),
		sdktrace.WithResource(res),
	)
	
	// Golang OpenTelemetry paketine tp ismindeki sağlayıcıyı kullanacağımızı bildirdik.
	otel.SetTracerProvider(tp)

	return &Tracer{
		tp: tp,
	}, nil
}


// Tracer'ın izlemesi için yeni bir katman oluşturma, böylelik aktif context altına yeni bir işlem eklenir.
// libName: user-service eg.
// spanName: get-user eg.
func (t *Tracer) StartSpan(ctx context.Context, libName, spanName string) (context.Context, trace2.Span) {
	tr := t.tp.Tracer(libName)
	return tr.Start(ctx, spanName)
}


// Trace sağlayıcının sonlandırılması
func (t *Tracer) ShutDown(ctx context.Context) error {
	return t.tp.Shutdown(ctx)
}
```

## 3rd Party Router OpenTelemetry Trace Paketinin Kurulması

- Gofiber için -> https://github.com/gofiber/contrib/tree/main/otelfiber
- Golang-chi için -> https://github.com/riandyrn/otelchi

> örnek `main.go` dosyası

```go
var (
		url         = "http://localhost:9411/api/v2/spans" // zipkin url
		serviceName = "duyurubu-panel"
		tracer      *Tracer
		err         error
	)

    // tracer init
	if tracer, err = NewTracer(url, serviceName); err != nil {
		log.Fatalln(err)
	}

	defer func() {
		if err := tracer.ShutDown(context.Background()); err != nil {
			log.Fatal("failed to shutdown TracerProvider: %w", err)
		}
	}()

	repository := NewRepository(tracer)

	service := NewService(repository, tracer)

	handler := NewHandler(service, tracer)

	// middleware setup
	r := chi.NewRouter()
	r.Use(otelchi.Middleware("duyurubu-panel-api", otelchi.WithChiRoutes(r)))

	r.Post("/login", handler.Login)

	log.Fatalln(http.ListenAndServe(":4444", r))
```

## Ek tracelerin eklenmesi

Tracelerin izlenmesi sadece handler'lar ile bitmiyor olabilir.

Aynı context üzerinden oluşturulmuş olan trace'ler Zipkin'de bir grup veya alt grup olarak görüntülenebilir. Bu yüzden aynı trace gurubunda olmasını istediğimiz işlemleri aynı context üzerinden yapmalıyız.

### Yeni Span Ekleme

```go
CustomServiceFunc(ctx, args...)
```

```go
func (s *Service) CustomServiceFunc(ctx contextContext, args...){
	ctx, span := s.tracer.StartSpan(s.libName, "custom-service-func") // yeni span başlattık.
	// ctx'i bir yere göndermeyeceksek blank olarak alabiliriz.
	defer span.End() // fonksiyon sonunda span'ı sonlandırdık. 
	
	// diğer işlemler
}
```



