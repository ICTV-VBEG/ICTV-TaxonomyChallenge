# Why do we need a computational taxonomy?

There is a consensus that viruses are so diverse that no single
taxonomic method can be used to classify them all (Simmonds et
al. PLoS Biology 2023). Since its inception, the ICTV has been seeking
the expertise of the global virology community to classify viruses in
accordance with their domain-specific knowledge. This has generated a
patchwork of methods that, ideally, capture the features of different
viral lineages and generate meaningful taxa that are in agreement with
biology. These methods are formalised in taxonomy proposals
(taxoprops) written by experts and ratified by the ICTV. These
documents describe how viruses within each taxon shall be classified,
and include specific demarcation criteria. They are available as Word
documents on the ICTV website.

As metagenomics is rapidly expanding our view of the virosphere, we
are looking to make sense of the sequences we discover. The number and
diversity of sequences found in viromics dataset is staggering and
make their taxonomic classification a daunting task that one would
ideally automate. There is currently no ICTV-approved method to
approach this question. While the solution will likely not be trivial,
we have to face this challenge to keep up with the growth of viruses
that we aim to classify.

# The methodology

We collected viral sequences that experts have classified into the
various ranks of the ICTV taxonomy. These sequences are available as a
multifasta file here. The challenge asks you to classify these
sequences using your pipeline and submit your results to us for
validation. We only ask that your pipeline be reproducible, i.e., that
the code and environment necessary to run it be made
available. Multiple strategies exist, such as the creation of virtual
environments (venv, conda) or containers (singularity, docker, etc.)
and the pipeline should be made available via a git repository
(github, bitbucket).

# The dataset

The fasta file is available here. We ask that your pipeline should
return a csv file where each entry (or as many as you can), follows
the following structure:

<div class="table-wrapper">
<table>
	<thead>
		<tr>
			<th> </th>
			<th>col_name1</th>
			<th>col_name2</th>
			<th>col_name3</th>
			<th>col_name4</th>
			<th>col_name5</th>
			<th>col_name6</th>
			<th>col_name7</th>
			<th>col_name8</th>
			<th>col_name9</th>
			<th>col_name10</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>row1</td>
			<td> </td>
			<td> </td>
			<td> </td>
			<td> </td>
			<td> </td>
			<td> </td>
			<td> </td>
			<td> </td>
			<td> </td>
			<td> </td>
		</tr>
		<tr>
			<td>row2</td>
			<td> </td>
			<td> </td>
			<td> </td>
			<td> </td>
			<td> </td>
			<td> </td>
			<td> </td>
			<td> </td>
			<td> </td>
			<td> </td>
		</tr>
	</tbody>
</table>

<!--|SequenceID|Realm|Subrealm|Kingom|Subkingdom|Phylum|Subphylum|Class|Subclass|Order|Suborder|Family|Subfamily|Genus|Subgenus|Species|
|:---------|:----|:-------|:-----|:---------|:-----|:--------|:----|:-------|:----|:-------|:-----|:--------|:----|:-------|:------|
|ICTVTaxoChallenge_XXXXX|Varidnaviria||Bamfordvirae||Nucleocytoviricota||Megaviricetes||Imitervirales||Mimiviridae|Megamimivirinae|Mimivirus||Mimivirus bradfordmassiliense| -->

</div>
