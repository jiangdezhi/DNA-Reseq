# samtools学习计划

## 1.samtools 基本参数

## 2.samtools flags

![samtools flagstat](flagstat.png)

    total：bam文件所有alignment数（即bam文件行数）,包括没有比对到参考基因组的、secondary和supplementary alignment，所以总行数大于或等于fastq的read总数。(分为QC-passed reads和 QC-failed reads两类)，与samtools view -c得到结果相同
    secondary: secondary alignment数，由于reads的multiple mapping产生的，与samtools view -f 256 得到结果相同
    supplementary: supplementary alignment数，由于chimeric reads产生的，与samtools view -f 2048得到结果相同
    duplicates:PCR重复？？
    mapped：比对上参考基因组的alignment数(该数占bam文件所有alignment的比列），包含secondary和supplementary alignment，与比对到基因组的read数是不一样的，与samtools view -F 4得到的结果相同。
    paired in sequencing：bam文件中成对的reads总数，包括比对上和没有对上的read（注：不是aligment数）
    read1：bam文件中属于reads1的reads数量
    read2：bam文件中属于reads2的reads数量
    properly paired：比对到基因组上正确配对的reads数量（即read1和read2都比对到同一染色体上，同时insert size在正常范围内。弄清楚代码原理），与samtools view -f 2得到结果相同
    with itself and mate mapped：比对到基因组上配对的reads数，包括read1和read2比对到不同染色体上或者insert size较大的成对的read数。
    singletons：只有单条reads比对上的reads数
    以上计数均以reads条数计，一对reads计为两条。

## 3.samtools cigar

## 4.samtools tags 

## 5.samtools source code 
