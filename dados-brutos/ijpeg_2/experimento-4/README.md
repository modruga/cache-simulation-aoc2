# comandos utilizados para o experimento 4

## blocos de 32 bytes, mapeamento direto

## o comando abaixo descreve uma cache separada entre dados e instruções em mapeamento direto com blocos de 32 bytes e 32 conjuntos cada

### `./sim-cache -cache:il1 il1:32:32:1:r -cache:dl1 dl1:32:32:1:r -cache:il2 none -cache:dl2 none -tlb:itlb none -tlb:dtlb none ./ijpeg.ss -image_file ./specmun.ppm -compression.quality 90 -compression.optimize_coding 0 -compression.smoothing_factor 90 -difference.image 1 -difference.x_stride 10 -difference.y_stride 10 -verbose 1 -GO.findoptcomp`

## blocos de 64 bytes, mapeamento direto

## o comando abaixo descreve uma cache separada entre dados e instruções em mapeamento direto com blocos de 64 bytes e 16 conjuntos cada

### `./sim-cache -cache:il1 il1:16:64:1:r -cache:dl1 dl1:16:64:1:r -cache:il2 none -cache:dl2 none -tlb:itlb none -tlb:dtlb none ./ijpeg.ss -image_file ./specmun.ppm -compression.quality 90 -compression.optimize_coding 0 -compression.smoothing_factor 90 -difference.image 1 -difference.x_stride 10 -difference.y_stride 10 -verbose 1 -GO.findoptcomp`

## blocos de 128 bytes, mapeamento direto

## o comando abaixo descreve uma cache separada entre dados e instruções em mapeamento direto com blocos de 128 bytes e 8 conjuntos cada

### `./sim-cache -cache:il1 il1:8:128:1:r -cache:dl1 dl1:8:128:1:r -cache:il2 none -cache:dl2 none -tlb:itlb none -tlb:dtlb none ./ijpeg.ss -image_file ./specmun.ppm -compression.quality 90 -compression.optimize_coding 0 -compression.smoothing_factor 90 -difference.image 1 -difference.x_stride 10 -difference.y_stride 10 -verbose 1 -GO.findoptcomp`

## blocos de 256 bytes, mapeamento direto

## o comando abaixo descreve uma cache separada entre dados e instruções em mapeamento direto com blocos de 256 bytes e 4 conjuntos cada

### `./sim-cache -cache:il1 il1:4:256:1:r -cache:dl1 dl1:4:256:1:r -cache:il2 none -cache:dl2 none -tlb:itlb none -tlb:dtlb none ./ijpeg.ss -image_file ./specmun.ppm -compression.quality 90 -compression.optimize_coding 0 -compression.smoothing_factor 90 -difference.image 1 -difference.x_stride 10 -difference.y_stride 10 -verbose 1 -GO.findoptcomp`
