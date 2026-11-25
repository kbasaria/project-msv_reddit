---
layout: slide
title: ""
---

## CROSS-VALIDATION MODEL COMPARISON

<div style="font-size:0.65em;color:#a6bfc4;margin:10px 0 22px;">
  Five-fold stratified cross-validation · Selected model configurations
</div>

<table style="width:100%;border-collapse:collapse;font-size:0.75em;margin:16px 0 26px;">
  <thead>
    <tr style="background:#174858;color:#fff;">
      <th style="padding:14px 10px;text-align:left;">MODEL</th>
      <th style="padding:14px 8px;text-align:center;">ACCURACY</th>
      <th style="padding:14px 8px;text-align:center;">SENSITIVITY</th>
      <th style="padding:14px 8px;text-align:center;">SPECIFICITY</th>
      <th style="padding:14px 8px;text-align:center;">ROC-AUC</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="padding:14px 10px;">Baseline LR</td>
      <td style="text-align:center;">.793</td>
      <td style="text-align:center;">.997</td>
      <td style="text-align:center;">.170</td>
      <td style="text-align:center;">.933</td>
    </tr>
    <tr>
      <td style="padding:14px 10px;">Weighted LR</td>
      <td style="text-align:center;">.882</td>
      <td style="text-align:center;">.905</td>
      <td style="text-align:center;">.810</td>
      <td style="text-align:center;">.934</td>
    </tr>
    <tr style="background:#123d4a;">
      <td style="padding:14px 10px;font-weight:bold;color:#fff;">Tuned BERT</td>
      <td style="text-align:center;font-weight:bold;color:#fff;">.916</td>
      <td style="text-align:center;">.948</td>
      <td style="text-align:center;">.820</td>
      <td style="text-align:center;">.953</td>
    </tr>
    <tr style="background:#174858;">
      <td style="padding:14px 10px;font-weight:bold;color:#fff;">Tuned RoBERTa</td>
      <td style="text-align:center;">.914</td>
      <td style="text-align:center;">.944</td>
      <td style="text-align:center;">.820</td>
      <td style="text-align:center;font-weight:bold;color:#fff;">.963</td>
    </tr>
  </tbody>
</table>

<div style="display:flex;gap:14px;margin:20px 0;">

  <div style="flex:1;background:#174858;border-radius:9px;padding:18px;text-align:center;">
    <div style="font-size:0.6em;color:#d5e7eb;">HIGHEST CV ACCURACY</div>
    <div style="font-size:1.5em;font-weight:bold;color:#fff;">91.6%</div>
    <div style="font-size:0.65em;color:#a6bfc4;">Tuned BERT</div>
  </div>

  <div style="flex:1;background:#174858;border-radius:9px;padding:18px;text-align:center;">
    <div style="font-size:0.6em;color:#d5e7eb;">HIGHEST ROC-AUC</div>
    <div style="font-size:1.5em;font-weight:bold;color:#fff;">0.963</div>
    <div style="font-size:0.65em;color:#a6bfc4;">Tuned RoBERTa</div>
  </div>

</div>

<div style="background:#174858;border-left:5px solid #64b5c4;border-radius:7px;padding:16px 20px;margin-top:18px;">

  <div style="font-size:0.65em;font-weight:bold;color:#fff;margin-bottom:6px;">
    KEY TAKEAWAY
  </div>

  <div style="font-size:0.7em;color:#d5e7eb;">
    RoBERTa was selected based on sensitivity-constrained threshold optimization, prioritizing the identification of survivor narratives.
  </div>

</div>
